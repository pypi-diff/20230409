# Comparing `tmp/robotcode_language_server-0.32.3.tar.gz` & `tmp/robotcode_language_server-0.33.0.tar.gz`

## Comparing `robotcode_language_server-0.32.3.tar` & `robotcode_language_server-0.33.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/lsp_types.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9178 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18305 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63852 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83660 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80204 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    39775 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/README.md
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/pyproject.toml
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 robotcode_language_server-0.32.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/lsp_types.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21125 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19025 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63852 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83656 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80273 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/discovering.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40456 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/README.md
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/pyproject.toml
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 robotcode_language_server-0.33.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/lsp_types.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/lsp_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/text_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,60 @@
 import weakref
 from typing import Any, Awaitable, Callable, Dict, Final, List, Optional, TypeVar, Union, cast
 
 from robotcode.core.async_tools import async_event, create_sub_task
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.core.uri import Uri
 
-from .lsp_types import DocumentUri, Range
+from .lsp_types import DocumentUri, Position, Range
+
+
+def is_multibyte_char(char: str) -> bool:
+    return ord(char) > 0xFFFF
+
+
+def position_from_utf16(lines: List[str], position: Position) -> Position:
+    if position.line >= len(lines):
+        return position
+
+    utf32_offset = 0
+    utf16_counter = 0
+
+    for c in lines[position.line]:
+        utf16_counter += 2 if is_multibyte_char(c) else 1
+
+        if utf16_counter > position.character:
+            break
+
+        utf32_offset += 1
+
+    return Position(line=position.line, character=utf32_offset)
+
+
+def position_to_utf16(lines: List[str], position: Position) -> Position:
+    if position.line >= len(lines):
+        return position
+
+    utf16_counter = 0
+
+    for i, c in enumerate(lines[position.line]):
+        if i >= position.character:
+            break
+
+        utf16_counter += 2 if is_multibyte_char(c) else 1
+
+    return Position(line=position.line, character=utf16_counter)
+
+
+def range_from_utf16(lines: List[str], range: Range) -> Range:
+    return Range(start=position_from_utf16(lines, range.start), end=position_from_utf16(lines, range.end))
+
+
+def range_to_utf16(lines: List[str], range: Range) -> Range:
+    return Range(start=position_to_utf16(lines, range.start), end=position_to_utf16(lines, range.end))
 
 
 class InvalidRangeError(Exception):
     pass
 
 
 _T = TypeVar("_T")
@@ -111,15 +156,15 @@
                     self._version = version
 
                 if range.start > range.end:
                     raise InvalidRangeError(f"Start position is greater then end position {range}.")
 
                 lines = self.__get_lines()
 
-                (start_line, start_col), (end_line, end_col) = range
+                (start_line, start_col), (end_line, end_col) = range_from_utf16(lines, range)
 
                 if start_line == len(lines):
                     self._text = self._text + text
                     return
 
                 with io.StringIO() as new_text:
                     for i, line in enumerate(lines):
@@ -255,7 +300,19 @@
         self._invalidate_cache()
         self._invalidate_data()
 
     @_logger.call
     def clear(self) -> None:
         with self._lock:
             self._clear()
+
+    def position_from_utf16(self, position: Position) -> Position:
+        return position_from_utf16(self.get_lines(), position)
+
+    def position_to_utf16(self, position: Position) -> Position:
+        return position_to_utf16(self.get_lines(), position)
+
+    def range_from_utf16(self, range: Range) -> Range:
+        return range_from_utf16(self.get_lines(), range)
+
+    def range_to_utf16(self, range: Range) -> Range:
+        return range_to_utf16(self.get_lines(), range)
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,32 +71,38 @@
     ) -> Optional[List[Union[Command, CodeAction]]]:
         results: List[Union[Command, CodeAction]] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
+        for c in context.diagnostics:
+            c.range = document.range_from_utf16(c.range)
+            if c.related_information is not None:
+                for r in c.related_information:
+                    r.location.range = document.range_from_utf16(r.location.range)
+
         for result in await self.collect(
             self,
             document,
-            range,
+            document.range_from_utf16(range),
             context,
             callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.extend(result)
 
-        if len(results) > 0:
-            return results
+        if not results:
+            return None
 
-        return None
+        return results
 
     @rpc_method(name="textDocument/codeAction/resolve", param_type=CodeAction)
     @threaded()
     async def _text_document_code_action_resolve(
         self,
         params: CodeAction,
         *args: Any,
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,18 +57,21 @@
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.extend(result)
 
-        if len(results) > 0:
-            return results
+        if not results:
+            return None
 
-        return None
+        for result in results:
+            result.range = document.range_to_utf16(result.range)
+
+        return results
 
     @rpc_method(name="codeLens/resolve", param_type=CodeLens)
     @threaded()
     async def _code_lens_resolve(self, params: CodeLens, *args: Any, **kwargs: Any) -> CodeLens:
         results: List[CodeLens] = []
 
         for result in await self.resolve(self, params):
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.lsp_types import (
     CompletionContext,
     CompletionItem,
     CompletionList,
     CompletionOptions,
     CompletionParams,
+    InsertReplaceEdit,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
+    TextEdit,
 )
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
@@ -85,42 +87,60 @@
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect(
             self,
             document,
-            position,
+            document.position_from_utf16(position),
             context,
             callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.append(result)
 
-        if len(results) > 0:
-            if any(e for e in results if isinstance(e, CompletionList)):
-                result = CompletionList(
-                    is_incomplete=any(e for e in results if isinstance(e, CompletionList) and e.is_incomplete),
-                    items=list(chain(*[r.items if isinstance(r, CompletionList) else r for r in results])),
-                )
-                if len(result.items) == 0:
-                    return None
-                return result
+        if not results:
+            return None
 
-            result = list(chain(*[k for k in results if isinstance(k, list)]))
-            if len(result) == 0:
+        for result in results:
+            if isinstance(result, CompletionList):
+                for item in result.items:
+                    if item.text_edit is not None:
+                        self.update_completion_item_to_utf16(document, item)
+
+            elif isinstance(result, list):
+                for item in result:
+                    if item.text_edit is not None:
+                        self.update_completion_item_to_utf16(document, item)
+
+        if any(e for e in results if isinstance(e, CompletionList)):
+            result = CompletionList(
+                is_incomplete=any(e for e in results if isinstance(e, CompletionList) and e.is_incomplete),
+                items=list(chain(*[r.items if isinstance(r, CompletionList) else r for r in results])),
+            )
+            if len(result.items) == 0:
                 return None
-
             return result
 
-        return None
+        result = list(chain(*[k for k in results if isinstance(k, list)]))
+        if not result:
+            return None
+
+        return result
+
+    def update_completion_item_to_utf16(self, document: TextDocument, item: CompletionItem) -> None:
+        if isinstance(item.text_edit, TextEdit):
+            item.text_edit.range = document.range_to_utf16(item.text_edit.range)
+        elif isinstance(item.text_edit, InsertReplaceEdit):
+            item.text_edit.insert = document.range_to_utf16(item.text_edit.insert)
+            item.text_edit.replace = document.range_to_utf16(item.text_edit.replace)
 
     @rpc_method(name="completionItem/resolve", param_type=CompletionItem)
     @threaded()
     async def _completion_item_resolve(
         self,
         params: CompletionItem,
         *args: Any,
@@ -132,14 +152,15 @@
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.append(result)
 
-        if len(results) > 0:
-            if len(results) > 1:
-                self._logger.warning("More then one resolve result. Use the last one.")
+        if not results:
+            return params
 
-            return results[-1]
+        if len(results) > 1:
+            self._logger.warning("More then one resolve result. Use the last one.")
+        result = results[-1]
 
-        return params
+        return result
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional, Union
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.lsp_types import (
-    DeclarationParams,
+    DefinitionParams,
     Location,
     LocationLink,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
 from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 
-class DeclarationProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
+class DefinitionProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
     _logger: Final = LoggingDescriptor()
 
     def __init__(self, parent: LanguageServerProtocol) -> None:
         super().__init__(parent)
         self.link_support = False
 
     @async_tasking_event
@@ -38,54 +36,68 @@
     ) -> Union[Location, List[Location], List[LocationLink], None]:
         ...
 
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if (
             self.parent.client_capabilities is not None
             and self.parent.client_capabilities.text_document is not None
-            and self.parent.client_capabilities.text_document.declaration
+            and self.parent.client_capabilities.text_document.definition
         ):
-            self.link_support = self.parent.client_capabilities.text_document.declaration.link_support or False
+            self.link_support = self.parent.client_capabilities.text_document.definition.link_support or False
 
         if len(self.collect):
-            capabilities.declaration_provider = True
+            capabilities.definition_provider = True
 
-    @rpc_method(name="textDocument/declaration", param_type=DeclarationParams)
+    @rpc_method(name="textDocument/definition", param_type=DefinitionParams)
     @threaded()
-    async def _text_document_declaration(
-        self,
-        text_document: TextDocumentIdentifier,
-        position: Position,
-        *args: Any,
-        **kwargs: Any,
+    async def _text_document_definition(
+        self, text_document: TextDocumentIdentifier, position: Position, *args: Any, **kwargs: Any
     ) -> Optional[Union[Location, List[Location], List[LocationLink]]]:
         locations: List[Location] = []
         location_links: List[LocationLink] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, position, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self, document, document.position_from_utf16(position), callback_filter=language_id_filter(document)
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     if isinstance(result, Location):
                         locations.append(result)
                     else:
                         for e in result:
                             if isinstance(e, Location):
                                 locations.append(e)
                             elif isinstance(e, LocationLink):
                                 location_links.append(e)
+
         if len(locations) == 0 and len(location_links) == 0:
             return None
 
+        if locations:
+            for location in locations:
+                doc = await self.parent.documents.get(location.uri)
+                if doc is not None:
+                    location.range = doc.range_to_utf16(location.range)
+
+        if location_links:
+            for location_link in location_links:
+                doc = await self.parent.documents.get(location_link.target_uri)
+                if doc is not None:
+                    location_link.target_range = doc.range_to_utf16(location_link.target_range)
+                    location_link.target_selection_range = doc.range_to_utf16(location_link.target_selection_range)
+                if location_link.origin_selection_range is not None:
+                    location_link.origin_selection_range = document.range_to_utf16(location_link.origin_selection_range)
+
         if len(locations) > 0 and len(location_links) == 0:
             if len(locations) == 1:
                 return locations[0]
 
             return locations
 
         if len(locations) > 0 and len(location_links) > 0:
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,24 @@
                     continue
                 if result_any is None:
                     continue
 
                 result = cast(DiagnosticsResult, result_any)
 
                 data.id = str(uuid.uuid4())
+
+                if result.diagnostics is not None:
+                    for d in result.diagnostics:
+                        d.range = document.range_to_utf16(d.range)
+
+                        for r in d.related_information or []:
+                            doc = await self.parent.documents.get(r.location.uri)
+                            if doc is not None:
+                                r.location.range = doc.range_to_utf16(r.location.range)
+
                 data.entries[result.key] = result.diagnostics
                 if result.diagnostics is not None:
                     collected_keys.append(result.key)
 
                 if data.entries and send_diagnostics:
                     self.parent.send_notification(
                         "textDocument/publishDiagnostics",
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,24 @@
     ) -> Optional[List[DocumentHighlight]]:
         highlights: List[DocumentHighlight] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, position, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self, document, document.position_from_utf16(position), callback_filter=language_id_filter(document)
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     highlights.extend(result)
 
         if len(highlights) == 0:
             return None
 
+        for highlight in highlights:
+            highlight.range = document.range_to_utf16(highlight.range)
+
         return highlights
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     async def _text_document_symbol(
         self, text_document: TextDocumentIdentifier, *args: Any, **kwargs: Any
     ) -> Optional[Union[List[DocumentSymbol], List[SymbolInformation], None]]:
         document_symbols: List[DocumentSymbol] = []
         symbol_informations: List[SymbolInformation] = []
 
         document = await self.parent.documents.get(text_document.uri)
-        if not document:
+        if document is None:
             return None
 
         for result in await self.collect(self, document, callback_filter=language_id_filter(document)):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
@@ -117,14 +117,30 @@
                         document_symbols.extend(result)
                     elif all(isinstance(e, SymbolInformation) for e in result):
                         symbol_informations.extend(result)
                     else:
                         self._logger.warning(
                             "Result contains DocumentSymbol and SymbolInformation results, result is skipped."
                         )
+        if document_symbols:
+
+            def traverse(symbol: DocumentSymbol, doc: TextDocument) -> None:
+                symbol.range = doc.range_to_utf16(symbol.range)
+                symbol.selection_range = doc.range_to_utf16(symbol.selection_range)
+                for child in symbol.children or []:
+                    traverse(child, doc)
+
+            for symbol in document_symbols:
+                traverse(symbol, document)
+
+        if symbol_informations:
+            for symbol_information in symbol_informations:
+                doc = await self.parent.documents.get(symbol_information.location.uri)
+                if doc is not None:
+                    symbol_information.location.range = doc.range_to_utf16(symbol_information.location.range)
 
         if document_symbols and symbol_informations:
             self._logger.warning(
                 "Result contains DocumentSymbol and SymbolInformation results, only DocumentSymbols returned."
             )
             return document_symbols
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,56 +3,79 @@
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
+from robotcode.language_server.common.has_extend_capabilities import (
+    HasExtendCapabilities,
+)
 from robotcode.language_server.common.lsp_types import (
-    FoldingRange,
-    FoldingRangeParams,
+    Hover,
+    HoverOptions,
+    HoverParams,
+    Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
-from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
+from robotcode.language_server.common.parts.protocol_part import (
+    LanguageServerProtocolPart,
+)
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
-    from robotcode.language_server.common.protocol import LanguageServerProtocol  # pragma: no cover
+    from robotcode.language_server.common.protocol import LanguageServerProtocol
 
 
-class FoldingRangeProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
+class HoverProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
     _logger: Final = LoggingDescriptor()
 
     def __init__(self, parent: LanguageServerProtocol) -> None:
         super().__init__(parent)
 
     @async_tasking_event
-    async def collect(sender, document: TextDocument) -> Optional[List[FoldingRange]]:  # pragma: no cover, NOSONAR
+    async def collect(sender, document: TextDocument, position: Position) -> Optional[Hover]:  # NOSONAR
         ...
 
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
-            capabilities.folding_range_provider = True
+            capabilities.hover_provider = HoverOptions(work_done_progress=True)
 
-    @rpc_method(name="textDocument/foldingRange", param_type=FoldingRangeParams)
+    @rpc_method(name="textDocument/hover", param_type=HoverParams)
     @threaded()
-    async def _text_document_folding_range(
-        self, text_document: TextDocumentIdentifier, *args: Any, **kwargs: Any
-    ) -> Optional[List[FoldingRange]]:
-        results: List[FoldingRange] = []
+    async def _text_document_hover(
+        self,
+        text_document: TextDocumentIdentifier,
+        position: Position,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Optional[Hover]:
+        results: List[Hover] = []
+
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self,
+            document,
+            document.position_from_utf16(position),
+            callback_filter=language_id_filter(document),
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
-                    results += result
+                    results.append(result)
 
-        if len(results) == 0:
-            return None
-        return results
+        for result in results:
+            if result.range is not None:
+                result.range = document.range_to_utf16(result.range)
+
+        if len(results) > 0 and results[-1].contents:
+            # TODO: how can we combine hover results?
+
+            return results[-1]
+
+        return None
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,75 +3,68 @@
 from asyncio import CancelledError
 from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.common.decorators import language_id_filter
-from robotcode.language_server.common.has_extend_capabilities import (
-    HasExtendCapabilities,
-)
+from robotcode.language_server.common.has_extend_capabilities import HasExtendCapabilities
 from robotcode.language_server.common.lsp_types import (
-    Hover,
-    HoverOptions,
-    HoverParams,
+    FoldingRange,
+    FoldingRangeParams,
     Position,
     ServerCapabilities,
     TextDocumentIdentifier,
 )
-from robotcode.language_server.common.parts.protocol_part import (
-    LanguageServerProtocolPart,
-)
+from robotcode.language_server.common.parts.protocol_part import LanguageServerProtocolPart
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
-    from robotcode.language_server.common.protocol import LanguageServerProtocol
+    from robotcode.language_server.common.protocol import LanguageServerProtocol  # pragma: no cover
 
 
-class HoverProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
+class FoldingRangeProtocolPart(LanguageServerProtocolPart, HasExtendCapabilities):
     _logger: Final = LoggingDescriptor()
 
     def __init__(self, parent: LanguageServerProtocol) -> None:
         super().__init__(parent)
 
     @async_tasking_event
-    async def collect(sender, document: TextDocument, position: Position) -> Optional[Hover]:  # NOSONAR
+    async def collect(sender, document: TextDocument) -> Optional[List[FoldingRange]]:  # pragma: no cover, NOSONAR
         ...
 
     def extend_capabilities(self, capabilities: ServerCapabilities) -> None:
         if len(self.collect):
-            capabilities.hover_provider = HoverOptions(work_done_progress=True)
+            capabilities.folding_range_provider = True
 
-    @rpc_method(name="textDocument/hover", param_type=HoverParams)
+    @rpc_method(name="textDocument/foldingRange", param_type=FoldingRangeParams)
     @threaded()
-    async def _text_document_hover(
-        self,
-        text_document: TextDocumentIdentifier,
-        position: Position,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Optional[Hover]:
-        results: List[Hover] = []
-
+    async def _text_document_folding_range(
+        self, text_document: TextDocumentIdentifier, *args: Any, **kwargs: Any
+    ) -> Optional[List[FoldingRange]]:
+        results: List[FoldingRange] = []
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(
-            self,
-            document,
-            position,
-            callback_filter=language_id_filter(document),
-        ):
+        for result in await self.collect(self, document, callback_filter=language_id_filter(document)):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
-                    results.append(result)
+                    results += result
 
-        if len(results) > 0 and results[-1].contents:
-            # TODO: can we combine hover results?
+        if not results:
+            return None
 
-            return results[-1]
+        for result in results:
+            if result.start_character is not None:
+                result.start_character = document.position_to_utf16(
+                    Position(result.start_line, result.start_character)
+                ).character
+            if result.end_character is not None:
+                result.end_character = document.position_to_utf16(
+                    Position(result.end_line, result.end_character)
+                ).character
 
-        return None
+        return results
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files 23% similar despite different names*

```diff
@@ -78,14 +78,29 @@
                             if isinstance(e, Location):
                                 locations.append(e)
                             elif isinstance(e, LocationLink):
                                 location_links.append(e)
         if len(locations) == 0 and len(location_links) == 0:
             return None
 
+        if locations:
+            for location in locations:
+                doc = await self.parent.documents.get(location.uri)
+                if doc is not None:
+                    location.range = doc.range_to_utf16(location.range)
+
+        if location_links:
+            for location_link in location_links:
+                doc = await self.parent.documents.get(location_link.target_uri)
+                if doc is not None:
+                    location_link.target_range = doc.range_to_utf16(location_link.target_range)
+                    location_link.target_selection_range = doc.range_to_utf16(location_link.target_selection_range)
+                if location_link.origin_selection_range is not None:
+                    location_link.origin_selection_range = document.range_to_utf16(location_link.origin_selection_range)
+
         if len(locations) > 0 and len(location_links) == 0:
             if len(locations) == 1:
                 return locations[0]
 
             return locations
 
         if len(locations) > 0 and len(location_links) > 0:
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,25 +59,29 @@
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect(
             self,
             document,
-            range,
+            document.range_from_utf16(range),
             callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.extend(result)
 
-        if len(results) > 0:
+        if results:
+            for result in results:
+                result.position = document.position_to_utf16(result.position)
+                # TODO: resolve
+
             return results
 
         return None
 
     @rpc_method(name="inlayHint/resolve", param_type=InlayHint)
     @threaded()
     async def _inlay_hint_resolve(
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from asyncio import CancelledError
-from typing import TYPE_CHECKING, Any, Final, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Final, List, Optional
 
 from robotcode.core.async_tools import async_tasking_event, threaded
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.jsonrpc2.protocol import rpc_method
 from robotcode.language_server.common.decorators import (
     HasLanguageId,
     language_id_filter,
@@ -15,15 +15,14 @@
 )
 from robotcode.language_server.common.lsp_types import (
     DocumentSelector,
     InlineValue,
     InlineValueContext,
     InlineValueParams,
     InlineValueRegistrationOptions,
-    Position,
     Range,
     ServerCapabilities,
     TextDocumentFilterType1,
     TextDocumentIdentifier,
 )
 from robotcode.language_server.common.parts.protocol_part import (
     LanguageServerProtocolPart,
@@ -62,35 +61,40 @@
             )
 
     @rpc_method(name="textDocument/inlineValue", param_type=InlineValueParams)
     @threaded()
     async def _text_document_inline_value(
         self,
         text_document: TextDocumentIdentifier,
-        range: Union[Range, List[Position]],
+        range: Range,
         context: InlineValueContext,
         *args: Any,
         **kwargs: Any,
     ) -> Optional[List[InlineValue]]:
         results: List[InlineValue] = []
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, range, context, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self, document, document.range_from_utf16(range), context, callback_filter=language_id_filter(document)
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results += result
 
-        if len(results) == 0:
+        if not results:
             return None
 
+        for result in results:
+            result.range = document.range_to_utf16(result.range)
+
         return results
 
     async def refresh(self) -> None:
         if (
             self.parent.client_capabilities
             and self.parent.client_capabilities.workspace
             and self.parent.client_capabilities.workspace.inline_value
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,18 +53,20 @@
         linked_ranges: List[Range] = []
         word_pattern: Optional[str] = None
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, position, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self, document, document.position_from_utf16(position), callback_filter=language_id_filter(document)
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     linked_ranges.extend(result.ranges)
                     if result.word_pattern is not None:
                         word_pattern = result.word_pattern
 
-        return LinkedEditingRanges(linked_ranges, word_pattern)
+        return LinkedEditingRanges([document.range_to_utf16(r) for r in linked_ranges], word_pattern)
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/references.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,20 +56,29 @@
         locations: List[Location] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect(
-            self, document, position, context, callback_filter=language_id_filter(document)
+            self,
+            document,
+            document.position_from_utf16(position),
+            context,
+            callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     locations.extend(result)
 
-        if len(locations) == 0:
+        if not locations:
             return None
 
+        for location in locations:
+            doc = await self.parent.documents.get(location.uri)
+            if doc is not None:
+                location.range = doc.range_to_utf16(location.range)
+
         return locations
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,17 +11,20 @@
     HasExtendCapabilities,
 )
 from robotcode.language_server.common.lsp_types import (
     ErrorCodes,
     Position,
     PrepareRenameParams,
     PrepareRenameResult,
+    PrepareRenameResultType1,
+    Range,
     RenameOptions,
     RenameParams,
     ServerCapabilities,
+    TextDocumentEdit,
     TextDocumentIdentifier,
     WorkspaceEdit,
 )
 from robotcode.language_server.common.text_document import TextDocument
 
 if TYPE_CHECKING:
     from robotcode.language_server.common.protocol import LanguageServerProtocol
@@ -72,28 +75,43 @@
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect(
             self,
             document,
-            position,
+            document.position_from_utf16(position),
             new_name,
             callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     edits.append(result)
 
-        if len(edits) == 0:
+        if not edits:
             return None
 
+        for we in edits:
+            if we.changes:
+                for uri, changes in we.changes.items():
+                    if changes:
+                        doc = await self.parent.documents.get(uri)
+                        for change in changes:
+                            if doc is not None:
+                                change.range = doc.range_to_utf16(change.range)
+            if we.document_changes:
+                for doc_change in [v for v in we.document_changes if isinstance(v, TextDocumentEdit)]:
+                    doc = await self.parent.documents.get(doc_change.text_document.uri)
+                    if doc is not None:
+                        for edit in doc_change.edits:
+                            edit.range = doc.range_to_utf16(edit.range)
+
         result = WorkspaceEdit()
         for we in edits:
             if we.changes:
                 if result.changes is None:
                     result.changes = {}
                 result.changes.update(we.changes)
 
@@ -121,23 +139,29 @@
         results: List[PrepareRenameResult] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect_prepare(
-            self, document, position, callback_filter=language_id_filter(document)
+            self, document, document.position_from_utf16(position), callback_filter=language_id_filter(document)
         ):
             if isinstance(result, BaseException):
                 if isinstance(result, CantRenameError):
                     raise JsonRPCErrorException(ErrorCodes.INVALID_PARAMS, str(result))
 
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.append(result)
 
-        if len(results) == 0:
+        if not results:
             return None
 
-        return results[-1]
+        result = results[-1]
+        if isinstance(result, Range):
+            result = document.range_to_utf16(result)
+        elif isinstance(result, PrepareRenameResultType1):
+            result.range = document.range_to_utf16(result.range)
+
+        return result
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,19 +51,32 @@
     ) -> Optional[List[SelectionRange]]:
         results: List[SelectionRange] = []
 
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
-        for result in await self.collect(self, document, positions, callback_filter=language_id_filter(document)):
+        for result in await self.collect(
+            self,
+            document,
+            [document.position_from_utf16(p) for p in positions],
+            callback_filter=language_id_filter(document),
+        ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
                 if result is not None:
                     results.extend(result)
 
-        if len(results) == 0:
+        if not results:
             return None
 
+        def traverse(selection_range: SelectionRange, doc: TextDocument) -> None:
+            selection_range.range = doc.range_to_utf16(selection_range.range)
+            if selection_range.parent is not None:
+                traverse(selection_range.parent, doc)
+
+        for result in results:
+            traverse(result, document)
+
         return results
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         document = await self.parent.documents.get(text_document.uri)
         if document is None:
             return None
 
         for result in await self.collect(
             self,
             document,
-            position,
+            document.position_from_utf16(position),
             context,
             callback_filter=language_id_filter(document),
         ):
             if isinstance(result, BaseException):
                 if not isinstance(result, CancelledError):
                     self._logger.exception(result, exc_info=result)
             else:
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,19 @@
     async def show_document(
         self,
         uri: URI,
         external: Optional[bool] = None,
         take_focus: Optional[bool] = None,
         selection: Optional[Range] = None,
     ) -> bool:
+        if selection is not None:
+            doc = await self.parent.documents.get(uri)
+            if doc is not None:
+                selection = doc.range_to_utf16(selection)
+
         r = await self.parent.send_request_async(
             "window/showDocument",
             ShowDocumentParams(uri=uri, external=external, take_focus=take_focus, selection=selection),
             ShowDocumentResult,
         )
         return r.success if r is not None else False
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     FileOperationPattern,
     FileOperationRegistrationOptions,
     FileRename,
     FileSystemWatcher,
     RenameFilesParams,
     ServerCapabilities,
     ServerCapabilitiesWorkspaceType,
+    TextDocumentEdit,
     TextEdit,
     WatchKind,
     WorkspaceEdit,
     WorkspaceFoldersChangeEvent,
     WorkspaceFoldersServerCapabilities,
 )
 from robotcode.language_server.common.lsp_types import (
@@ -505,14 +506,28 @@
                     and self.parent.client_capabilities.workspace.did_change_watched_files
                     and self.parent.client_capabilities.workspace.did_change_watched_files.dynamic_registration
                 ):
                     await self.parent.unregister_capability(entry.id, "workspace/didChangeWatchedFiles")
                 # TODO: implement own filewatcher if not supported by language server client
 
     async def apply_edit(self, edit: WorkspaceEdit, label: Optional[str] = None) -> ApplyWorkspaceEditResult:
+        if edit.changes:
+            for uri, changes in edit.changes.items():
+                if changes:
+                    doc = await self.parent.documents.get(uri)
+                    for change in changes:
+                        if doc is not None:
+                            change.range = doc.range_to_utf16(change.range)
+        if edit.document_changes:
+            for doc_change in [v for v in edit.document_changes if isinstance(v, TextDocumentEdit)]:
+                doc = await self.parent.documents.get(doc_change.text_document.uri)
+                if doc is not None:
+                    for e in doc_change.edits:
+                        e.range = doc.range_to_utf16(e.range)
+
         r = await self.parent.send_request_async(
             "workspace/applyEdit",
             ApplyWorkspaceEditParams(edit, label),
             return_type=ApplyWorkspaceEditResult,
         )
 
         assert r is not None
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1722,15 +1722,15 @@
                 return cached[0]
 
             try:
                 result = self._find_keyword(name)
                 if result is None:
                     self.diagnostics.append(
                         DiagnosticsEntry(
-                            f"No keyword with name {repr(name)} found.",
+                            f"No keyword with name '{name}' found.",
                             DiagnosticSeverity.ERROR,
                             "KeywordNotFoundError",
                         )
                     )
             except KeywordError as e:
                 if raise_keyword_error:
                     raise
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,23 @@
 
 
 KEYWORD_WITH_ARGS_TEMPLATE = Template(
     """\
 ${name}
     [Arguments]    ${args}
     Fail
+
 """
 )
 
 KEYWORD_TEMPLATE = Template(
     """\
 ${name}
     Fail
+
 """
 )
 
 
 class FindKeywordSectionVisitor(AsyncVisitor):
     def __init__(self) -> None:
         self.keyword_sections: List[ast.AST] = []
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -938,15 +938,19 @@
                             return await self.create_headers_completion_items(r)
 
         elif position.character == 0:
             return await self.create_headers_completion_items(None)
 
         if len(nodes_at_position) > 1 and isinstance(nodes_at_position[0], HasTokens):
             node = nodes_at_position[0]
+
             tokens_at_position = get_tokens_at_position(node, position)
+            if not tokens_at_position:
+                return None
+
             token_at_position = tokens_at_position[-1]
 
             if isinstance(node, Arguments):
                 arg = self.get_variable_token(token_at_position)
                 if arg is not None and position <= range_from_token(arg).end:
                     return None
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/discovering.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/discovering.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
             return [
                 TextEdit(
                     range=Range(
                         start=Position(line=0, character=0),
                         end=Position(
                             line=len(document.get_lines()),
-                            character=len((document.get_lines())[-1]),
+                            character=0,
                         ),
                     ),
                     new_text=new.text,
                 )
             ]
 
         except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
@@ -197,15 +197,15 @@
 
             return [
                 TextEdit(
                     range=Range(
                         start=Position(line=0, character=0),
                         end=Position(
                             line=len(document.get_lines()),
-                            character=len((document.get_lines())[-1]),
+                            character=0,
                         ),
                     ),
                     new_text=s.getvalue(),
                 )
             ]
 
     @language_id("robotframework")
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     cast,
 )
 
 from robotcode.core.async_itertools import async_dropwhile, async_takewhile
 from robotcode.core.logging import LoggingDescriptor
 from robotcode.language_server.common.decorators import language_id
 from robotcode.language_server.common.lsp_types import (
+    Position,
     Range,
     SemanticTokenModifiers,
     SemanticTokens,
     SemanticTokensDelta,
     SemanticTokensDeltaPartialResult,
     SemanticTokensPartialResult,
     SemanticTokenTypes,
 )
-from robotcode.language_server.common.text_document import TextDocument
+from robotcode.language_server.common.text_document import TextDocument, range_to_utf16
 from robotcode.language_server.robotframework.diagnostics.library_doc import (
     ALL_RUN_KEYWORDS_MATCHERS,
     BUILTIN_LIBRARY_NAME,
     KeywordArgumentKind,
     KeywordDoc,
     KeywordMatcher,
     LibraryDoc,
@@ -305,15 +306,15 @@
                             last_index - 2,
                         )
 
                         yield SemTokenInfo(
                             token.lineno, col_offset + last_index, 1, RobotSemTokenTypes.VARIABLE_END, sem_mod
                         )
 
-                        if length - last_index > 0:
+                        if length - last_index - 1 > 0:
                             yield SemTokenInfo.from_token(
                                 token, sem_type, sem_mod, col_offset + last_index + 1, length - last_index - 1
                             )
                     else:
                         yield SemTokenInfo.from_token(token, sem_type, sem_mod)
 
                 else:
@@ -736,14 +737,15 @@
                         continue
 
             yield token, node
 
     @_logger.call
     async def _collect_internal(
         self,
+        document: TextDocument,
         model: ast.AST,
         range: Optional[Range],
         namespace: Namespace,
         builtin_library_doc: Optional[LibraryDoc],
         libraries_matchers: Dict[KeywordMatcher, LibraryEntry],
         resources_matchers: Dict[KeywordMatcher, ResourceEntry],
     ) -> Union[SemanticTokens, SemanticTokensPartialResult, None]:
@@ -843,43 +845,58 @@
                                     yield kw_res
 
                                 continue
 
                     for token in node.tokens:
                         yield token, node
 
+        lines = document.get_lines()
+
         async for robot_token, robot_node in async_takewhile(
             lambda t: range is None or token_in_range(t[0], range),
             async_dropwhile(
                 lambda t: range is not None and not token_in_range(t[0], range),
                 (
                     (t, n)
                     async for t, n in get_tokens()
                     if t.type not in [RobotToken.SEPARATOR, RobotToken.EOL, RobotToken.EOS]
                 ),
             ),
         ):
             async for token in self.generate_sem_tokens(
                 robot_token, robot_node, namespace, builtin_library_doc, libraries_matchers, resources_matchers
             ):
+                if token.length == 0:
+                    continue
+
+                token_range = range_to_utf16(
+                    lines,
+                    Range(
+                        start=Position(line=token.lineno - 1, character=token.col_offset),
+                        end=Position(line=token.lineno - 1, character=token.col_offset + token.length),
+                    ),
+                )
+                token_col_offset = token_range.start.character
+                token_length = token_range.end.character - token_range.start.character
+
                 current_line = token.lineno - 1
 
                 data.append(current_line - last_line)
 
                 if last_line != current_line:
-                    last_col = token.col_offset
+                    last_col = token_col_offset
                     data.append(last_col)
                 else:
-                    delta = token.col_offset - last_col
+                    delta = token_col_offset - last_col
                     data.append(delta)
                     last_col += delta
 
                 last_line = current_line
 
-                data.append(token.length)
+                data.append(token_length)
 
                 data.append(self.parent.semantic_tokens.token_types.index(token.sem_token_type))
 
                 data.append(
                     reduce(
                         operator.or_,
                         (2 ** self.parent.semantic_tokens.token_modifiers.index(e) for e in token.sem_modifiers),
@@ -905,14 +922,15 @@
                 and library.import_name == BUILTIN_LIBRARY_NAME
                 and library.import_range == Range.zero()
             ),
             None,
         )
 
         return await self._collect_internal(
+            document,
             model,
             range,
             namespace,
             builtin_library_doc,
             await namespace.get_libraries_matchers(),
             await namespace.get_resources_matchers(),
         )
```

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.33.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/.gitignore` & `robotcode_language_server-0.33.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/LICENSE.txt` & `robotcode_language_server-0.33.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/README.md` & `robotcode_language_server-0.33.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/pyproject.toml` & `robotcode_language_server-0.33.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.32.3/PKG-INFO` & `robotcode_language_server-0.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.32.3
+Version: 0.33.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
```

