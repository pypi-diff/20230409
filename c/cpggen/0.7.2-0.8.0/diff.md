# Comparing `tmp/cpggen-0.7.2.tar.gz` & `tmp/cpggen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.7.2.tar", max compression
+gzip compressed data, was "cpggen-0.8.0.tar", max compression
```

## Comparing `cpggen-0.7.2.tar` & `cpggen-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-09 18:02:12.315227 cpggen-0.7.2/LICENSE
--rw-r--r--   0        0        0     5622 2023-04-09 18:02:12.315227 cpggen-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-04-09 18:02:12.315227 cpggen-0.7.2/cpggen/__init__.py
--rw-r--r--   0        0        0     8290 2023-04-09 18:02:12.315227 cpggen-0.7.2/cpggen/cli.py
--rw-r--r--   0        0        0    16565 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/executor.py
--rw-r--r--   0        0        0      731 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/logger.py
--rw-r--r--   0        0        0     9682 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-09 18:02:12.319227 cpggen-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 cpggen-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-09 21:17:58.868180 cpggen-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6474 2023-04-09 21:17:58.868180 cpggen-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/__init__.py
+-rw-r--r--   0        0        0    12106 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/cli.py
+-rw-r--r--   0        0        0    18921 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/executor.py
+-rw-r--r--   0        0        0      731 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/logger.py
+-rw-r--r--   0        0        0     9682 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-09 21:17:58.872180 cpggen-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 cpggen-0.8.0/PKG-INFO
```

### Comparing `cpggen-0.7.2/LICENSE` & `cpggen-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.2/README.md` & `cpggen-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
@@ -95,14 +95,30 @@
 
 Container based invocation
 
 ```
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
+### Export graphs
+
+By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
+
+Example to export `all` graphs in `dot` format
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
+```
+
+To export `pdg` in `neo4jcsv` format
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out --export-repr pdg --export-format neo4jcsv
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -153,14 +169,17 @@
 | JOERN_HOME              | Joern installation directory                                      |
 | CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
 | CPGGEN_PORT             | cpggen server port. Default 7072                                  |
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
+| CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
+| CPG_EXPORT_REPR         | Graph to export. Default all                                      |
+| CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-0.7.2/cpggen/cli.py` & `cpggen-0.8.0/cpggen/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
+import json
 import os
+import shutil
 import signal
 import tempfile
 from multiprocessing import Pool
 from pathlib import Path
 
 from quart import Quart, request
 
@@ -37,15 +39,15 @@
     """
     parser = argparse.ArgumentParser(description="CPG Generator")
     parser.add_argument(
         "-i", "--src", dest="src", help="Source directory or url", default=os.getcwd()
     )
     parser.add_argument(
         "-o",
-        "--out_dir",
+        "--out-dir",
         dest="cpg_out_dir",
         help="CPG output directory",
         default=os.path.join(os.getcwd(), "cpg_out"),
     )
     parser.add_argument(
         "-l",
         "--lang",
@@ -113,14 +115,41 @@
     )
     parser.add_argument(
         "--server-port",
         default=os.getenv("CPGGEN_PORT", "7072"),
         dest="server_port",
         help="cpggen server port",
     )
+    parser.add_argument(
+        "--export",
+        action="store_true",
+        default=True if os.getenv("CPG_EXPORT") in ("true", "1") else False,
+        dest="export",
+        help="Export CPG as a graph",
+    )
+    parser.add_argument(
+        "--export-repr",
+        default=os.getenv("CPG_EXPORT_REPR", "all"),
+        dest="export_repr",
+        choices=["ast", "cfg", "cdg", "ddg", "pdg", "cpg", "all"],
+        help="Graph representation to export",
+    )
+    parser.add_argument(
+        "--export-format",
+        default=os.getenv("CPG_EXPORT_FORMAT", "dot"),
+        dest="export_format",
+        choices=["neo4jcsv", "graphml", "graphson", "dot"],
+        help="Export format",
+    )
+    parser.add_argument(
+        "--export-out-dir",
+        default=os.path.join(os.getcwd(), "export_out"),
+        dest="export_out_dir",
+        help="Export output directoru",
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -218,22 +247,86 @@
                             lang,
                             src,
                             cpg_out_dir,
                             src,
                             joern_home,
                             use_container,
                             auto_build,
+                            {},
                         ),
                     )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
+def collect_cpg_manifests(cpg_out_dir):
+    return utils.find_files(cpg_out_dir, ".manifest.json")
+
+
+def export_cpg(
+    src,
+    cpg_out_dir,
+    joern_home,
+    use_container,
+    export_repr,
+    export_format,
+    export_out_dir,
+):
+    if __name__ in ("__main__", "cpggen.cli"):
+        with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
+            try:
+                cpg_manifests = collect_cpg_manifests(cpg_out_dir)
+                for amanifest in cpg_manifests:
+                    with open(amanifest) as mfp:
+                        manifest_obj = json.load(mfp)
+                        if not manifest_obj or not manifest_obj.get("cpg"):
+                            continue
+                        app_export_out_dir = os.path.join(
+                            export_out_dir, manifest_obj["app"]
+                        )
+                        try:
+                            # joern-export annoyingly will not overwrite directories
+                            # but would expect first level directories to exist
+                            if os.path.exists(app_export_out_dir):
+                                try:
+                                    shutil.rmtree(app_export_out_dir)
+                                except Exception:
+                                    # Ignore remove errors
+                                    pass
+                            os.makedirs(export_out_dir, exist_ok=True)
+                        except Exception:
+                            # Ignore errors
+                            pass
+                        LOG.debug(
+                            f"""Exporting CPG for the app {manifest_obj["app"]} to {app_export_out_dir}"""
+                        )
+                        pool.apply_async(
+                            executor.exec_tool,
+                            (
+                                "export",
+                                manifest_obj["cpg"],
+                                app_export_out_dir,
+                                cpg_out_dir,
+                                joern_home,
+                                use_container,
+                                False,
+                                {
+                                    "export_repr": export_repr,
+                                    "export_format": export_format,
+                                },
+                            ),
+                        )
+                pool.close()
+            except KeyboardInterrupt:
+                pool.terminate()
+            pool.join()
+
+
 def main():
     print(product_logo)
     args = build_args()
     if args.server_mode:
         return run_server(args)
     src = args.src
     cpg_out_dir = args.cpg_out_dir
@@ -269,17 +362,27 @@
         src,
         cpg_out_dir,
         languages,
         joern_home=joern_home,
         use_container=use_container,
         auto_build=args.auto_build,
     )
+    if args.export:
+        export_cpg(
+            src,
+            cpg_out_dir,
+            joern_home=joern_home,
+            use_container=use_container,
+            export_repr=args.export_repr,
+            export_format=args.export_format,
+            export_out_dir=args.export_out_dir,
+        )
     if is_temp_dir:
         try:
-            os.remove(src)
+            shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cpggen-0.7.2/cpggen/executor.py` & `cpggen-0.8.0/cpggen/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
     "jar": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "cdxgen -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
+    "export": "joern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
         "maven": [
             get("MVN_CMD", "mvn"),
@@ -179,14 +180,15 @@
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
     joern_home=None,
     use_container=False,
     auto_build=False,
+    extra_args={},
     env=os.environ.copy(),
     stdout=subprocess.DEVNULL,
 ):
     with Progress(
         console=console,
         transient=True,
         redirect_stderr=False,
@@ -195,18 +197,21 @@
     ) as progress:
         task = None
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
         try:
             stderr = subprocess.DEVNULL
             if LOG.isEnabledFor(DEBUG):
-                stderr = subprocess.STDOUT
-            tool_verb = "Building CPG with"
+                stdout = subprocess.PIPE
+                stderr = stdout
+            tool_verb = f"Building CPG with {tool_lang} frontend"
+            if tool_lang == "export":
+                tool_verb = "Exporting CPG with joern-export"
             task = progress.add_task(
-                "[green]" + tool_verb + " " + tool_lang + " frontend",
+                "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
             cmd_with_args = cpg_tools_map.get(tool_lang)
             if not cmd_with_args:
                 return
             uber_jar = ""
@@ -238,64 +243,105 @@
                     container_cli = "docker"
                     if check_command("podman"):
                         container_cli = "podman"
                     cmd_with_args = f"""{container_cli} run --rm -w {amodule} -v {tempfile.gettempdir()}:/tmp -v {amodule}:{amodule}:rw -v {os.path.abspath(cpg_out_dir)}:{os.path.abspath(cpg_out_dir)}:rw -t {os.getenv("CPGGEN_IMAGE", "ghcr.io/appthreat/cpggen")} {cmd_with_args}"""
                     # We need to fix joern_home to the directory inside the container
                     joern_home = ""
                 sbom_cmd_with_args = cpg_tools_map.get("sbom")
-                cpg_out = (
-                    cpg_out_dir
-                    if cpg_out_dir.endswith(".bin.zip")
-                    or cpg_out_dir.endswith(".bin")
-                    or cpg_out_dir.endswith(".cpg")
-                    else os.path.join(
-                        cpg_out_dir,
-                        f"{os.path.basename(amodule)}-{tool_lang}-cpg.bin.zip",
+                sbom_out = ""
+                manifest_out = ""
+                if tool_lang == "export":
+                    cpg_out = cpg_out_dir
+                else:
+                    cpg_out = (
+                        cpg_out_dir
+                        if cpg_out_dir.endswith(".bin.zip")
+                        or cpg_out_dir.endswith(".bin")
+                        or cpg_out_dir.endswith(".cpg")
+                        else os.path.join(
+                            cpg_out_dir,
+                            f"{os.path.basename(amodule)}-{tool_lang}-cpg.bin.zip",
+                        )
                     )
-                )
-                sbom_out = (
-                    cpg_out.replace(".bin.zip", ".bom.xml")
-                    if cpg_out.endswith(".bin.zip")
-                    else f"{cpg_out}.bom.xml"
-                )
-                manifest_out = (
-                    cpg_out.replace(".bin.zip", ".manifest.json")
-                    if cpg_out.endswith(".bin.zip")
-                    else f"{cpg_out}.manifest.json"
-                )
-                LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
+                    sbom_out = (
+                        cpg_out.replace(".bin.zip", ".bom.xml")
+                        if cpg_out.endswith(".bin.zip")
+                        else f"{cpg_out}.bom.xml"
+                    )
+                    manifest_out = (
+                        cpg_out.replace(".bin.zip", ".manifest.json")
+                        if cpg_out.endswith(".bin.zip")
+                        else f"{cpg_out}.manifest.json"
+                    )
+                    LOG.debug(f"CPG file for {tool_lang} is {cpg_out}")
                 cmd_with_args = cmd_with_args % dict(
                     src=amodule,
                     cpg_out=cpg_out,
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
+                    **extra_args,
                 )
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
-                    src=amodule,
-                    tool_lang=tool_lang,
-                    sbom_out=sbom_out,
+                    src=amodule, tool_lang=tool_lang, sbom_out=sbom_out, **extra_args
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
                 if not check_command(lang_cmd):
                     if not use_container:
                         LOG.warn(
                             f"{lang_cmd} is not found. Try running cpggen with --use-container argument"
                         )
                     else:
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
                         )
                     return
+                # Is this an Export task?
+                if tool_lang == "export":
+                    try:
+                        cp = subprocess.run(
+                            cmd_list_with_args,
+                            stdout=stdout,
+                            stderr=stderr,
+                            cwd=cwd,
+                            env=env,
+                            check=False,
+                            shell=False,
+                            encoding="utf-8",
+                        )
+                        if cp and cp.returncode and cp.stderr:
+                            LOG.warn(f"Export CPG has failed for {src}")
+                            if cp.stdout:
+                                LOG.info(cp.stdout)
+                            if cp.stderr:
+                                LOG.info("------------------------------")
+                                LOG.info(cp.stderr)
+                                LOG.info("------------------------------")
+                                LOG.info(
+                                    "Please report the above error to https://github.com/joernio/joern/issues"
+                                )
+                        else:
+                            if os.path.exists(src):
+                                LOG.info(
+                                    f"CPG {src} successfully exported to {cpg_out_dir}"
+                                )
+                            else:
+                                LOG.warn(
+                                    f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually"
+                                )
+                    except Exception:
+                        LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
+                    progress.update(task, completed=100, total=100)
+                    continue
                 LOG.debug(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
                     )
                 )
@@ -326,21 +372,19 @@
                     check=False,
                     shell=False,
                     encoding="utf-8",
                 )
                 if cp and stdout == subprocess.PIPE:
                     for line in cp.stdout:
                         progress.update(task, completed=5)
-                if (
-                    cp
-                    and LOG.isEnabledFor(DEBUG)
-                    and cp.returncode
-                    and cp.stdout is not None
-                ):
-                    LOG.debug(cp.stdout)
+                if cp and LOG.isEnabledFor(DEBUG) and cp.returncode:
+                    if cp.stdout:
+                        LOG.debug(cp.stdout)
+                    if cp.stderr:
+                        LOG.debug(cp.stderr)
                 progress.update(task, completed=100, total=100)
                 if os.path.exists(cpg_out):
                     # go2cpg seems to produce a cpg without read permissions
                     try:
                         os.chmod(cpg_out, 0o644)
                     except Exception:
                         # Ignore errors
```

### Comparing `cpggen-0.7.2/cpggen/logger.py` & `cpggen-0.8.0/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.2/cpggen/utils.py` & `cpggen-0.8.0/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.2/pyproject.toml` & `cpggen-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.7.2"
+version = "0.8.0"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.7.2/PKG-INFO` & `cpggen-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.7.2
+Version: 0.8.0
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -70,23 +70,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
@@ -127,14 +127,30 @@
 
 Container based invocation
 
 ```
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
 
+### Export graphs
+
+By passing `--export`, cpggen can export the various graphs to many formats using [joern-export](https://docs.joern.io/exporting/)
+
+Example to export `all` graphs in `dot` format
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out
+```
+
+To export `pdg` in `neo4jcsv` format
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/export_out --export-repr pdg --export-format neo4jcsv
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -185,14 +201,17 @@
 | JOERN_HOME              | Joern installation directory                                      |
 | CPGGEN_HOST             | cpggen server host. Default 127.0.0.1                             |
 | CPGGEN_PORT             | cpggen server port. Default 7072                                  |
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
+| CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
+| CPG_EXPORT_REPR         | Graph to export. Default all                                      |
+| CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

