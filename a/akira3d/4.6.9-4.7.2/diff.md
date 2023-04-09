# Comparing `tmp/akira3d-4.6.9.tar.gz` & `tmp/akira3d-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akira3d-4.6.9.tar", last modified: Mon Mar 27 07:32:31 2023, max compression
+gzip compressed data, was "akira3d-4.7.2.tar", last modified: Sun Apr  9 19:25:28 2023, max compression
```

## Comparing `akira3d-4.6.9.tar` & `akira3d-4.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 07:32:31.762618 akira3d-4.6.9/
--rw-rw-rw-   0        0        0      144 2023-03-27 07:32:31.762618 akira3d-4.6.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-27 07:32:31.758617 akira3d-4.6.9/akira3d/
--rw-rw-rw-   0        0        0      489 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/camera.py
--rw-rw-rw-   0        0        0     4879 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/colliders.py
--rw-rw-rw-   0        0        0      366 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/gameEngine.py
--rw-rw-rw-   0        0        0      505 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/light.py
--rw-rw-rw-   0        0        0      277 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/mesh.py
--rw-rw-rw-   0        0        0     1329 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/mobs.py
--rw-rw-rw-   0        0        0     7234 2023-03-27 07:23:35.000000 akira3d-4.6.9/akira3d/model.py
--rw-rw-rw-   0        0        0     1248 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/phisics.py
--rw-rw-rw-   0        0        0     6942 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/render.py
--rw-rw-rw-   0        0        0      868 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/shader_program.py
--rw-rw-rw-   0        0        0     2627 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/texture.py
--rw-rw-rw-   0        0        0     1413 2023-03-27 07:25:20.000000 akira3d-4.6.9/akira3d/vao.py
--rw-rw-rw-   0        0        0     5087 2023-03-27 07:21:19.000000 akira3d-4.6.9/akira3d/vbo.py
--rw-rw-rw-   0        0        0     2082 2023-03-26 08:11:01.000000 akira3d-4.6.9/akira3d/vidSys.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:32:31.761618 akira3d-4.6.9/akira3d.egg-info/
--rw-rw-rw-   0        0        0      144 2023-03-27 07:32:31.000000 akira3d-4.6.9/akira3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-03-27 07:32:31.000000 akira3d-4.6.9/akira3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 07:32:31.000000 akira3d-4.6.9/akira3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-27 07:32:31.000000 akira3d-4.6.9/akira3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-03-27 07:32:31.000000 akira3d-4.6.9/akira3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 07:32:31.762618 akira3d-4.6.9/setup.cfg
--rw-rw-rw-   0        0        0      241 2023-03-27 07:29:25.000000 akira3d-4.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.607980 akira3d-4.7.2/
+-rw-rw-rw-   0        0        0      144 2023-04-09 19:25:28.607980 akira3d-4.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.603979 akira3d-4.7.2/akira3d/
+-rw-rw-rw-   0        0        0      489 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/__init__.py
+-rw-rw-rw-   0        0        0     2073 2023-04-09 18:03:38.000000 akira3d-4.7.2/akira3d/camera.py
+-rw-rw-rw-   0        0        0     4879 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/colliders.py
+-rw-rw-rw-   0        0        0      366 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/gameEngine.py
+-rw-rw-rw-   0        0        0      505 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/light.py
+-rw-rw-rw-   0        0        0      277 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/mesh.py
+-rw-rw-rw-   0        0        0     1329 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/mobs.py
+-rw-rw-rw-   0        0        0     7713 2023-04-09 19:23:39.000000 akira3d-4.7.2/akira3d/model.py
+-rw-rw-rw-   0        0        0     1248 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/phisics.py
+-rw-rw-rw-   0        0        0     6942 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/render.py
+-rw-rw-rw-   0        0        0      882 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/shader_program.py
+-rw-rw-rw-   0        0        0     2785 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/texture.py
+-rw-rw-rw-   0        0        0     1413 2023-03-27 07:34:49.000000 akira3d-4.7.2/akira3d/vao.py
+-rw-rw-rw-   0        0        0     5094 2023-04-09 17:25:55.000000 akira3d-4.7.2/akira3d/vbo.py
+-rw-rw-rw-   0        0        0     2097 2023-04-09 17:24:56.000000 akira3d-4.7.2/akira3d/vidSys.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:25:28.606981 akira3d-4.7.2/akira3d.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-09 19:25:28.000000 akira3d-4.7.2/akira3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:25:28.607980 akira3d-4.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-04-09 19:25:23.000000 akira3d-4.7.2/setup.py
```

### Comparing `akira3d-4.6.9/akira3d/camera.py` & `akira3d-4.7.2/akira3d/camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import glm
 import pygame as pg
 
 
 class Camera:
     def __init__(self, app, position=(0,0,4), yaw=-90, pitch=0):
         self.app = app
+        self.rotMouse = [0, 0]
+        self.visible = True
+        self.cinematog = False
+        self.pcm = {True:[0.02, 0.94], False:[0.15, 0.5]}
         self.aspect_ratio = app.size[0] / app.size[1]
         self.position = glm.vec3(position)
         self.up = glm.vec3(0, 1, 0)
         self.right = glm.vec3(1, 0, 0)
         self.forward = glm.vec3(0, 0, -1)
         self.yaw = yaw
         self.pitch = pitch
-        self.FOV = 80
-        self.NEAR = 0.3
-        self.FAR = 100
+        self.ini(80, 0.1, 10000)
         self.px, self.pn = 90, -90
 
+    def ini(self, fov, near, far):
+        self.FOV = fov
+        self.NEAR = near
+        self.FAR = far
         self.gvm()
         self.gpm()
 
-    def rotate(self, angle):
-        if angle != None:
-            self.yaw +=  angle[0]
-            self.pitch -=  angle[1]
-            self.pitch = max(self.pn, min(self.px, self.pitch))
+    def rot(self, rel):
+        self.rotMouse[0] += rel[0] * self.pcm[self.cinematog][0]
+        self.rotMouse[1] += rel[1] * self.pcm[self.cinematog][0]
 
     def ucv(self):
         yaw, pitch = glm.radians(self.yaw), glm.radians(self.pitch)
-
         self.forward.x = glm.cos(yaw) * glm.cos(pitch)
         self.forward.y = glm.sin(pitch)
         self.forward.z = glm.sin(yaw) * glm.cos(pitch)
-
         self.forward = glm.normalize(self.forward)
         self.right = glm.normalize(glm.cross(self.forward, glm.vec3(0,1,0)))
         self.up = glm.normalize(glm.cross(self.right, self.forward))
 
-    def update(self, pos=None, angle=None):
-        self.move(pos)
-        self.rotate(angle)
+    def update(self):
         self.ucv()
         self.gvm()
+        self.yaw += self.rotMouse[0]
+        self.pitch -= self.rotMouse[1]
+        self.pitch = max(self.pn, min(self.px, self.pitch))
+        self.rotMouse = [i * self.pcm[self.cinematog][1] for i in self.rotMouse]
 
-    def move(self, pos):
-        if pos != None: self.position = pos
-
+    def vis(self): self.visible = not self.visible; pg.mouse.set_visible(self.visible); pg.event.set_grab(not(self.visible));
+    def cin(self): self.cinematog = not self.cinematog
     def gvm(self): self.m_view = glm.lookAt(self.position, self.position + self.forward, self.up)
     def gpm(self): self.m_proj = glm.perspective(glm.radians(self.FOV), self.aspect_ratio, self.NEAR, self.FAR)
```

### Comparing `akira3d-4.6.9/akira3d/colliders.py` & `akira3d-4.7.2/akira3d/colliders.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.6.9/akira3d/mobs.py` & `akira3d-4.7.2/akira3d/mobs.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.6.9/akira3d/model.py` & `akira3d-4.7.2/akira3d/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,24 +72,31 @@
 
     def update(self):
         self.texture.use(location=0)
         [vao[0].program['camPos'].write(self.app.camera.position) for vao in self.vao.vaos]
         [vao[0].program['m_view'].write(self.app.camera.m_view) for vao in self.vao.vaos]
         [vao[0].program['m_model'].write(self.m_model) for vao in self.vao.vaos]
 
+        [vao[1].program['m_proj'].write(self.camera.m_proj) for vao in self.vao.vaos]
+        [vao[1].program['m_view_light'].write(self.app.light.m_view_light) for vao in self.vao.vaos]
+
+        [vao[0].program['m_proj'].write(self.app.camera.m_proj) for vao in self.vao.vaos]
+        #fog = max(min((glm.distance(self.app.camera.position, self.pos) - 100)/20, 1.0), 0);
+        #print(fog)
+        #[vao[0].program['fog'].write(glm.float64(fog)) for vao in self.vao.vaos]
+
     def update_shadow(self):
         [vao[1].program['m_model'].write(self.m_model) for vao in self.vao.vaos]
 
     def render_shadow(self):
         self.update_shadow()
         [vao[1].render() for vao in self.vao.vaos]
 
     def on_init(self):
         [vao[0].program['m_view_light'].write(self.app.light.m_view_light) for vao in self.vao.vaos]
-
         [vao[0].program['u_resolution'].write(glm.vec2(self.app.size)) for vao in self.vao.vaos]
 
         self.depth_texture = self.app.mesh.texture.textures['dt']
         for vao in self.vao.vaos: vao[0].program['shadowMap'] = 1
         self.depth_texture.use(location=1)
 
         [vao[1].program['m_proj'].write(self.camera.m_proj) for vao in self.vao.vaos]
@@ -99,15 +106,14 @@
         self.texture = self.app.mesh.texture.gt(self.tex_id)
         for vao in self.vao.vaos: vao[0].program['u_texture_0'] = 0
         self.texture.use(location=0)
 
         [vao[0].program['m_proj'].write(self.app.camera.m_proj) for vao in self.vao.vaos]
         [vao[0].program['m_view'].write(self.app.camera.m_view) for vao in self.vao.vaos]
         [vao[0].program['m_model'].write(self.m_model) for vao in self.vao.vaos]
-
         [vao[0].program['light.position'].write(self.app.light.position) for vao in self.vao.vaos]
         [vao[0].program['light.Ia'].write(self.app.light.Ia) for vao in self.vao.vaos]
         [vao[0].program['light.Id'].write(self.app.light.Id) for vao in self.vao.vaos]
         [vao[0].program['light.Is'].write(self.app.light.Is) for vao in self.vao.vaos]
 
     def tex(self, name=None, tex=None):
         self.tex_id = name
```

### Comparing `akira3d-4.6.9/akira3d/phisics.py` & `akira3d-4.7.2/akira3d/phisics.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.6.9/akira3d/render.py` & `akira3d-4.7.2/akira3d/render.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.6.9/akira3d/shader_program.py` & `akira3d-4.7.2/akira3d/shader_program.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,18 @@
         self.programs = {}
         self.programs['default'] = self.get_program('default')
         self.programs['skybox'] = self.get_program('skybox')
         self.programs['advanced_skybox'] = self.get_program('advanced_skybox')
         self.programs['shadow_map'] = self.get_program('shadow_map')
 
     def get_program(self, shader_program_name):
-        with open(f'shaders/{shader_program_name}.vert') as file:
+        with open(f'accets/shaders/{shader_program_name}.vert') as file:
             vertex_shader = file.read()
 
-        with open(f'shaders/{shader_program_name}.frag') as file:
+        with open(f'accets/shaders/{shader_program_name}.frag') as file:
             fragment_shader = file.read()
 
         program = self.ctx.program(vertex_shader=vertex_shader, fragment_shader=fragment_shader)
         return program
 
     def destroy(self):
         [program.release() for program in self.programs.values()]
```

### Comparing `akira3d-4.6.9/akira3d/texture.py` & `akira3d-4.7.2/akira3d/texture.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,33 @@
         self.textures = {'default':self.get_texture('default.png'), 'dt':self.get_depth_texture()}
         self.skyBoxes = {'default':self.get_texture_cube('default')}
 
     def loadTexPack(self, names):
         for name in names:
             self.textures[name] = self.get_texture(name)
 
+    def loadSkyPack(self, names):
+        for name in names:
+            self.skyBoxes[name] = self.get_texture_cube(name)
+
     def get_depth_texture(self):
         tex = self.ctx.depth_texture(self.app.size)
         tex.repeat_x = False
         tex.repeat_y = False
         return tex
 
     def get_texture_cube(self, name):
         faces = ['right', 'left', 'top', 'bottom'] + ['front', 'back'][::-1]
         textures = []
         for face in faces:
             texPath = ''
             if self.os == 'posix':
-                texPath = f'./skyboxes/{name}/{face}.png'
+                texPath = f'./accets/skyboxes/{name}/{face}.png'
             elif self.os == 'nt':
-                texPath = f'skyboxes\\{name}\\{face}.png'
+                texPath = f'accets\\skyboxes\\{name}\\{face}.png'
             texture = pg.image.load(texPath).convert_alpha()
             if face in ['right', 'left', 'front', 'back']:
                 texture = pg.transform.flip(texture, flip_x=True, flip_y=False)
             else:
                 texture = pg.transform.flip(texture, flip_x=False, flip_y=True)
             textures.append(texture)
         size = textures[0].get_size()
@@ -42,17 +46,17 @@
             texture_data = pg.image.tostring(textures[i], 'RGB')
             texture_cube.write(face=i, data=texture_data)
         return texture_cube
 
     def get_texture(self, name):
         texPath = ''
         if self.os == 'posix':
-            texPath = f'./textures/{name}'
+            texPath = f'./accets/textures/{name}'
         elif self.os == 'nt':
-            texPath = f'textures\\{name}'
+            texPath = f'accets\\textures\\{name}'
         img = pg.image.load(texPath).convert_alpha()
         return self.create_texture(img)
 
     def create_texture(self, img):
         img = pg.transform.flip(img, flip_x=False, flip_y=True)
         texture = self.ctx.texture(size=img.get_size(), components=4, data=pg.image.tostring(img, 'RGBA'))
         texture.filter = (mgl.LINEAR_MIPMAP_LINEAR, mgl.LINEAR)
```

### Comparing `akira3d-4.6.9/akira3d/vao.py` & `akira3d-4.7.2/akira3d/vao.py`

 * *Files identical despite different names*

### Comparing `akira3d-4.6.9/akira3d/vbo.py` & `akira3d-4.7.2/akira3d/vbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 system = os.name
 
 class VBO:
     def __init__(self, ctx):
         print('load models')
-        self.folder = Path('models')
+        self.folder = Path('accets/models')
         self.vbos = {}
         self.vbos1 = {}
         self.vbos['cube'] = CubeVBO(ctx)
         self.vbos1['skybox'] = SkyBoxVBO(ctx)
         self.vbos1['advanced_skybox'] = AdvancedSkyBoxVBO(ctx)
         for file in self.folder.iterdir():
             file = str(file)
```

### Comparing `akira3d-4.6.9/akira3d/vidSys.py` & `akira3d-4.7.2/akira3d/vidSys.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,14 @@
         self.app = app
         self.clips = {}
 
     def loadClipPack(self, datas):
         for data in datas:
             texPath = ''
             if data[0] != 0:
-                if self.os == 'posix': texPath = f'./clips/{data[0]}'
-                elif self.os == 'nt': texPath = f'clips\\{data[0]}'
+                if self.os == 'posix': texPath = f'./accets/clips/{data[0]}'
+                elif self.os == 'nt': texPath = f'accets\\clips\\{data[0]}'
             else: texPath = 0
             self.clips[data[1]] = Clip(texPath, data[2])
 
     def release(self):
         [clip.release() for clip in self.clips.values()]
```

