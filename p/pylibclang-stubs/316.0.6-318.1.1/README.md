# Comparing `tmp/pylibclang-stubs-316.0.6.tar.gz` & `tmp/pylibclang_stubs-318.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibclang-stubs-316.0.6.tar", last modified: Sat Oct 28 10:36:31 2023, max compression
+gzip compressed data, was "pylibclang_stubs-318.1.1.tar", last modified: Mon May 27 12:17:14 2024, max compression
```

## Comparing `pylibclang-stubs-316.0.6.tar` & `pylibclang_stubs-318.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-28 10:36:30.993343 pylibclang-stubs-316.0.6/
--rw-r--r--   0 edi       (1000) edi       (1000)      667 2023-10-28 10:36:30.993343 pylibclang-stubs-316.0.6/PKG-INFO
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-28 10:36:30.993343 pylibclang-stubs-316.0.6/pylibclang-stubs/
--rw-r--r--   0 edi       (1000) edi       (1000)   499543 2023-10-28 10:36:23.000000 pylibclang-stubs-316.0.6/pylibclang-stubs/_C.pyi
-drwxr-xr-x   0 edi       (1000) edi       (1000)        0 2023-10-28 10:36:30.993343 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/
--rw-r--r--   0 edi       (1000) edi       (1000)      667 2023-10-28 10:36:30.000000 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/PKG-INFO
--rw-r--r--   0 edi       (1000) edi       (1000)      237 2023-10-28 10:36:30.000000 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 edi       (1000) edi       (1000)        1 2023-10-28 10:36:30.000000 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 edi       (1000) edi       (1000)        1 2023-10-28 10:36:30.000000 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/not-zip-safe
--rw-r--r--   0 edi       (1000) edi       (1000)       17 2023-10-28 10:36:30.000000 pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/top_level.txt
--rw-r--r--   0 edi       (1000) edi       (1000)      994 2023-10-28 10:36:02.000000 pylibclang-stubs-316.0.6/pyproject.toml
--rw-r--r--   0 edi       (1000) edi       (1000)       38 2023-10-28 10:36:30.993343 pylibclang-stubs-316.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:17:14.971280 pylibclang_stubs-318.1.1/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-27 12:17:14.971280 pylibclang_stubs-318.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:17:14.961280 pylibclang_stubs-318.1.1/pylibclang-stubs/
+-rw-r--r--   0 root         (0) root         (0)   530470 2024-05-27 12:17:13.000000 pylibclang_stubs-318.1.1/pylibclang-stubs/_C.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 12:17:14.971280 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-27 12:17:14.000000 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-27 12:17:14.000000 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 12:17:14.000000 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 12:17:14.000000 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-27 12:17:14.000000 pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-27 12:15:10.000000 pylibclang_stubs-318.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 12:17:14.971280 pylibclang_stubs-318.1.1/setup.cfg
```

### Comparing `pylibclang-stubs-316.0.6/PKG-INFO` & `pylibclang_stubs-318.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibclang-stubs
-Version: 316.0.6
+Version: 318.1.1
 Summary: Python stubs for pylibclang
 License: MIT
 Project-URL: Homepage, https://github.com/edimetia3d/pylibclang
 Project-URL: Documentation, https://github.com/edimetia3d/pylibclang
 Project-URL: Repository, https://github.com/edimetia3d/pylibclang
 Project-URL: Changelog, https://github.com/edimetia3d/pylibclang/releases
 Keywords: pybind11,libclang,python,stubs
```

### Comparing `pylibclang-stubs-316.0.6/pylibclang-stubs/_C.pyi` & `pylibclang_stubs-318.1.1/pylibclang-stubs/_C.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 import typing
-__all__ = ['CXAPISetImplp', 'CXAPISetImplpp', 'CXAvailabilityKind', 'CXCallingConv', 'CXChildVisitResult', 'CXCodeCompleteResults', 'CXCodeComplete_Flags', 'CXComment', 'CXCommentInlineCommandRenderKind', 'CXCommentKind', 'CXCommentParamPassDirection', 'CXCompilationDatabase_Error', 'CXCompletionChunkKind', 'CXCompletionContext', 'CXCompletionResult', 'CXCursor', 'CXCursorAndRangeVisitor', 'CXCursorKind', 'CXCursorSetImplp', 'CXCursor_ExceptionSpecificationKind', 'CXCursorpp', 'CXDiagnosticDisplayOptions', 'CXDiagnosticSeverity', 'CXErrorCode', 'CXEvalResultKind', 'CXFileUniqueID', 'CXGlobalOptFlags', 'CXIdxAttrInfo', 'CXIdxAttrKind', 'CXIdxBaseClassInfo', 'CXIdxCXXClassDeclInfo', 'CXIdxContainerInfo', 'CXIdxDeclInfo', 'CXIdxDeclInfoFlags', 'CXIdxEntityCXXTemplateKind', 'CXIdxEntityInfo', 'CXIdxEntityKind', 'CXIdxEntityLanguage', 'CXIdxEntityRefInfo', 'CXIdxEntityRefKind', 'CXIdxIBOutletCollectionAttrInfo', 'CXIdxImportedASTFileInfo', 'CXIdxIncludedFileInfo', 'CXIdxLoc', 'CXIdxObjCCategoryDeclInfo', 'CXIdxObjCContainerDeclInfo', 'CXIdxObjCContainerKind', 'CXIdxObjCInterfaceDeclInfo', 'CXIdxObjCPropertyDeclInfo', 'CXIdxObjCProtocolRefInfo', 'CXIdxObjCProtocolRefListInfo', 'CXIndexOptFlags', 'CXLanguageKind', 'CXLinkageKind', 'CXLoadDiag_Error', 'CXModuleMapDescriptorImplp', 'CXNameRefFlags', 'CXObjCDeclQualifierKind', 'CXObjCPropertyAttrKind', 'CXPlatformAvailability', 'CXPrintingPolicyProperty', 'CXRefQualifierKind', 'CXReparse_Flags', 'CXResult', 'CXSaveError', 'CXSaveTranslationUnit_Flags', 'CXSourceLocation', 'CXSourceRange', 'CXSourceRangeList', 'CXString', 'CXStringSet', 'CXSymbolRole', 'CXTLSKind', 'CXTUResourceUsage', 'CXTUResourceUsageEntry', 'CXTUResourceUsageKind', 'CXTargetInfoImplp', 'CXTemplateArgumentKind', 'CXToken', 'CXTokenKind', 'CXTokenpp', 'CXTranslationUnitImplp', 'CXTranslationUnitImplpp', 'CXTranslationUnit_Flags', 'CXType', 'CXTypeKind', 'CXTypeLayoutError', 'CXTypeNullabilityKind', 'CXUnsavedFile', 'CXVersion', 'CXVirtualFileOverlayImplp', 'CXVisibilityKind', 'CXVisitorResult', 'CX_CXXAccessSpecifier', 'CX_StorageClass', 'IndexerCallbacks', 'StringHolder', 'TokenArray', 'charpp', 'clang_BlockCommandComment_getArgText', 'clang_BlockCommandComment_getCommandName', 'clang_BlockCommandComment_getNumArgs', 'clang_BlockCommandComment_getParagraph', 'clang_CXCursorSet_contains', 'clang_CXCursorSet_insert', 'clang_CXIndex_getGlobalOptions', 'clang_CXIndex_setGlobalOptions', 'clang_CXIndex_setInvocationEmissionPathOption', 'clang_CXRewriter_create', 'clang_CXRewriter_dispose', 'clang_CXRewriter_insertTextBefore', 'clang_CXRewriter_overwriteChangedFiles', 'clang_CXRewriter_removeText', 'clang_CXRewriter_replaceText', 'clang_CXRewriter_writeMainFileToStdOut', 'clang_CXXConstructor_isConvertingConstructor', 'clang_CXXConstructor_isCopyConstructor', 'clang_CXXConstructor_isDefaultConstructor', 'clang_CXXConstructor_isMoveConstructor', 'clang_CXXField_isMutable', 'clang_CXXMethod_isConst', 'clang_CXXMethod_isCopyAssignmentOperator', 'clang_CXXMethod_isDefaulted', 'clang_CXXMethod_isDeleted', 'clang_CXXMethod_isMoveAssignmentOperator', 'clang_CXXMethod_isPureVirtual', 'clang_CXXMethod_isStatic', 'clang_CXXMethod_isVirtual', 'clang_CXXRecord_isAbstract', 'clang_Comment_getChild', 'clang_Comment_getKind', 'clang_Comment_getNumChildren', 'clang_Comment_isWhitespace', 'clang_CompilationDatabase_dispose', 'clang_CompilationDatabase_fromDirectory', 'clang_CompilationDatabase_getAllCompileCommands', 'clang_CompilationDatabase_getCompileCommands', 'clang_CompileCommand_getArg', 'clang_CompileCommand_getDirectory', 'clang_CompileCommand_getFilename', 'clang_CompileCommand_getMappedSourceContent', 'clang_CompileCommand_getMappedSourcePath', 'clang_CompileCommand_getNumArgs', 'clang_CompileCommand_getNumMappedSources', 'clang_CompileCommands_dispose', 'clang_CompileCommands_getCommand', 'clang_CompileCommands_getSize', 'clang_Cursor_Evaluate', 'clang_Cursor_getArgument', 'clang_Cursor_getBriefCommentText', 'clang_Cursor_getCXXManglings', 'clang_Cursor_getCommentRange', 'clang_Cursor_getMangling', 'clang_Cursor_getModule', 'clang_Cursor_getNumArguments', 'clang_Cursor_getNumTemplateArguments', 'clang_Cursor_getObjCDeclQualifiers', 'clang_Cursor_getObjCManglings', 'clang_Cursor_getObjCPropertyAttributes', 'clang_Cursor_getObjCPropertyGetterName', 'clang_Cursor_getObjCPropertySetterName', 'clang_Cursor_getObjCSelectorIndex', 'clang_Cursor_getOffsetOfField', 'clang_Cursor_getParsedComment', 'clang_Cursor_getRawCommentText', 'clang_Cursor_getReceiverType', 'clang_Cursor_getSpellingNameRange', 'clang_Cursor_getStorageClass', 'clang_Cursor_getTemplateArgumentKind', 'clang_Cursor_getTemplateArgumentType', 'clang_Cursor_getTemplateArgumentUnsignedValue', 'clang_Cursor_getTemplateArgumentValue', 'clang_Cursor_getTranslationUnit', 'clang_Cursor_getVarDeclInitializer', 'clang_Cursor_hasAttrs', 'clang_Cursor_hasVarDeclExternalStorage', 'clang_Cursor_hasVarDeclGlobalStorage', 'clang_Cursor_isAnonymous', 'clang_Cursor_isAnonymousRecordDecl', 'clang_Cursor_isBitField', 'clang_Cursor_isDynamicCall', 'clang_Cursor_isExternalSymbol', 'clang_Cursor_isFunctionInlined', 'clang_Cursor_isInlineNamespace', 'clang_Cursor_isMacroBuiltin', 'clang_Cursor_isMacroFunctionLike', 'clang_Cursor_isNull', 'clang_Cursor_isObjCOptional', 'clang_Cursor_isVariadic', 'clang_EnumDecl_isScoped', 'clang_EvalResult_dispose', 'clang_EvalResult_getAsDouble', 'clang_EvalResult_getAsInt', 'clang_EvalResult_getAsLongLong', 'clang_EvalResult_getAsStr', 'clang_EvalResult_getAsUnsigned', 'clang_EvalResult_getKind', 'clang_EvalResult_isUnsignedInt', 'clang_File_isEqual', 'clang_File_tryGetRealPathName', 'clang_FullComment_getAsHTML', 'clang_FullComment_getAsXML', 'clang_HTMLStartTagComment_isSelfClosing', 'clang_HTMLStartTag_getAttrName', 'clang_HTMLStartTag_getAttrValue', 'clang_HTMLStartTag_getNumAttrs', 'clang_HTMLTagComment_getAsString', 'clang_HTMLTagComment_getTagName', 'clang_IndexAction_create', 'clang_IndexAction_dispose', 'clang_InlineCommandComment_getArgText', 'clang_InlineCommandComment_getCommandName', 'clang_InlineCommandComment_getNumArgs', 'clang_InlineCommandComment_getRenderKind', 'clang_InlineContentComment_hasTrailingNewline', 'clang_Location_isFromMainFile', 'clang_Location_isInSystemHeader', 'clang_ModuleMapDescriptor_create', 'clang_ModuleMapDescriptor_dispose', 'clang_ModuleMapDescriptor_setFrameworkModuleName', 'clang_ModuleMapDescriptor_setUmbrellaHeader', 'clang_ModuleMapDescriptor_writeToBuffer', 'clang_Module_getASTFile', 'clang_Module_getFullName', 'clang_Module_getName', 'clang_Module_getNumTopLevelHeaders', 'clang_Module_getParent', 'clang_Module_getTopLevelHeader', 'clang_Module_isSystem', 'clang_ParamCommandComment_getDirection', 'clang_ParamCommandComment_getParamIndex', 'clang_ParamCommandComment_getParamName', 'clang_ParamCommandComment_isDirectionExplicit', 'clang_ParamCommandComment_isParamIndexValid', 'clang_PrintingPolicy_dispose', 'clang_PrintingPolicy_getProperty', 'clang_PrintingPolicy_setProperty', 'clang_Range_isNull', 'clang_TParamCommandComment_getDepth', 'clang_TParamCommandComment_getIndex', 'clang_TParamCommandComment_getParamName', 'clang_TParamCommandComment_isParamPositionValid', 'clang_TargetInfo_dispose', 'clang_TargetInfo_getPointerWidth', 'clang_TargetInfo_getTriple', 'clang_TextComment_getText', 'clang_Type_getAlignOf', 'clang_Type_getCXXRefQualifier', 'clang_Type_getClassType', 'clang_Type_getModifiedType', 'clang_Type_getNamedType', 'clang_Type_getNullability', 'clang_Type_getNumObjCProtocolRefs', 'clang_Type_getNumObjCTypeArgs', 'clang_Type_getNumTemplateArguments', 'clang_Type_getObjCEncoding', 'clang_Type_getObjCObjectBaseType', 'clang_Type_getObjCProtocolDecl', 'clang_Type_getObjCTypeArg', 'clang_Type_getOffsetOf', 'clang_Type_getSizeOf', 'clang_Type_getTemplateArgumentAsType', 'clang_Type_getValueType', 'clang_Type_isTransparentTagTypedef', 'clang_Type_visitFields', 'clang_VerbatimBlockLineComment_getText', 'clang_VerbatimLineComment_getText', 'clang_VirtualFileOverlay_addFileMapping', 'clang_VirtualFileOverlay_create', 'clang_VirtualFileOverlay_dispose', 'clang_VirtualFileOverlay_setCaseSensitivity', 'clang_VirtualFileOverlay_writeToBuffer', 'clang_annotateTokens', 'clang_codeCompleteAt', 'clang_codeCompleteGetContainerKind', 'clang_codeCompleteGetContainerUSR', 'clang_codeCompleteGetContexts', 'clang_codeCompleteGetDiagnostic', 'clang_codeCompleteGetNumDiagnostics', 'clang_codeCompleteGetObjCSelector', 'clang_constructUSR_ObjCCategory', 'clang_constructUSR_ObjCClass', 'clang_constructUSR_ObjCIvar', 'clang_constructUSR_ObjCMethod', 'clang_constructUSR_ObjCProperty', 'clang_constructUSR_ObjCProtocol', 'clang_createAPISet', 'clang_createCXCursorSet', 'clang_createIndex', 'clang_createTranslationUnit', 'clang_createTranslationUnit2', 'clang_createTranslationUnitFromSourceFile', 'clang_defaultCodeCompleteOptions', 'clang_defaultDiagnosticDisplayOptions', 'clang_defaultEditingTranslationUnitOptions', 'clang_defaultReparseOptions', 'clang_defaultSaveOptions', 'clang_disposeAPISet', 'clang_disposeCXCursorSet', 'clang_disposeCXPlatformAvailability', 'clang_disposeCXTUResourceUsage', 'clang_disposeCodeCompleteResults', 'clang_disposeDiagnostic', 'clang_disposeDiagnosticSet', 'clang_disposeIndex', 'clang_disposeOverriddenCursors', 'clang_disposeSourceRangeList', 'clang_disposeString', 'clang_disposeStringSet', 'clang_disposeTokens', 'clang_disposeTranslationUnit', 'clang_enableStackTraces', 'clang_equalCursors', 'clang_equalLocations', 'clang_equalRanges', 'clang_equalTypes', 'clang_executeOnThread', 'clang_findIncludesInFile', 'clang_findReferencesInFile', 'clang_formatDiagnostic', 'clang_free', 'clang_getAddressSpace', 'clang_getAllSkippedRanges', 'clang_getArgType', 'clang_getArrayElementType', 'clang_getArraySize', 'clang_getBuildSessionTimestamp', 'clang_getCString', 'clang_getCXTUResourceUsage', 'clang_getCXXAccessSpecifier', 'clang_getCanonicalCursor', 'clang_getCanonicalType', 'clang_getChildDiagnostics', 'clang_getClangVersion', 'clang_getCompletionAnnotation', 'clang_getCompletionAvailability', 'clang_getCompletionBriefComment', 'clang_getCompletionChunkCompletionString', 'clang_getCompletionChunkKind', 'clang_getCompletionChunkText', 'clang_getCompletionFixIt', 'clang_getCompletionNumAnnotations', 'clang_getCompletionNumFixIts', 'clang_getCompletionParent', 'clang_getCompletionPriority', 'clang_getCursor', 'clang_getCursorAvailability', 'clang_getCursorCompletionString', 'clang_getCursorDefinition', 'clang_getCursorDisplayName', 'clang_getCursorExceptionSpecificationType', 'clang_getCursorExtent', 'clang_getCursorKind', 'clang_getCursorKindSpelling', 'clang_getCursorLanguage', 'clang_getCursorLexicalParent', 'clang_getCursorLinkage', 'clang_getCursorLocation', 'clang_getCursorPlatformAvailability', 'clang_getCursorPrettyPrinted', 'clang_getCursorPrintingPolicy', 'clang_getCursorReferenceNameRange', 'clang_getCursorReferenced', 'clang_getCursorResultType', 'clang_getCursorSemanticParent', 'clang_getCursorSpelling', 'clang_getCursorTLSKind', 'clang_getCursorType', 'clang_getCursorUSR', 'clang_getCursorVisibility', 'clang_getDeclObjCTypeEncoding', 'clang_getDefinitionSpellingAndExtent', 'clang_getDiagnostic', 'clang_getDiagnosticCategory', 'clang_getDiagnosticCategoryName', 'clang_getDiagnosticCategoryText', 'clang_getDiagnosticFixIt', 'clang_getDiagnosticInSet', 'clang_getDiagnosticLocation', 'clang_getDiagnosticNumFixIts', 'clang_getDiagnosticNumRanges', 'clang_getDiagnosticOption', 'clang_getDiagnosticRange', 'clang_getDiagnosticSetFromTU', 'clang_getDiagnosticSeverity', 'clang_getDiagnosticSpelling', 'clang_getElementType', 'clang_getEnumConstantDeclUnsignedValue', 'clang_getEnumConstantDeclValue', 'clang_getEnumDeclIntegerType', 'clang_getExceptionSpecificationType', 'clang_getExpansionLocation', 'clang_getFieldDeclBitWidth', 'clang_getFile', 'clang_getFileContents', 'clang_getFileLocation', 'clang_getFileName', 'clang_getFileTime', 'clang_getFileUniqueID', 'clang_getFunctionTypeCallingConv', 'clang_getIBOutletCollectionType', 'clang_getIncludedFile', 'clang_getInclusions', 'clang_getInstantiationLocation', 'clang_getLocation', 'clang_getLocationForOffset', 'clang_getModuleForFile', 'clang_getNonReferenceType', 'clang_getNullCursor', 'clang_getNullLocation', 'clang_getNullRange', 'clang_getNumArgTypes', 'clang_getNumCompletionChunks', 'clang_getNumDiagnostics', 'clang_getNumDiagnosticsInSet', 'clang_getNumElements', 'clang_getNumOverloadedDecls', 'clang_getOverloadedDecl', 'clang_getOverriddenCursors', 'clang_getPointeeType', 'clang_getPresumedLocation', 'clang_getRange', 'clang_getRangeEnd', 'clang_getRangeStart', 'clang_getRemappings', 'clang_getRemappingsFromFileList', 'clang_getResultType', 'clang_getSkippedRanges', 'clang_getSpecializedCursorTemplate', 'clang_getSpellingLocation', 'clang_getSymbolGraphForCursor', 'clang_getSymbolGraphForUSR', 'clang_getTUResourceUsageName', 'clang_getTemplateCursorKind', 'clang_getToken', 'clang_getTokenExtent', 'clang_getTokenKind', 'clang_getTokenLocation', 'clang_getTokenSpelling', 'clang_getTranslationUnitCursor', 'clang_getTranslationUnitSpelling', 'clang_getTranslationUnitTargetInfo', 'clang_getTypeDeclaration', 'clang_getTypeKindSpelling', 'clang_getTypeSpelling', 'clang_getTypedefDeclUnderlyingType', 'clang_getTypedefName', 'clang_getUnqualifiedType', 'clang_hashCursor', 'clang_indexLoc_getCXSourceLocation', 'clang_indexLoc_getFileLocation', 'clang_indexSourceFile', 'clang_indexSourceFileFullArgv', 'clang_indexTranslationUnit', 'clang_index_getCXXClassDeclInfo', 'clang_index_getClientContainer', 'clang_index_getClientEntity', 'clang_index_getIBOutletCollectionAttrInfo', 'clang_index_getObjCCategoryDeclInfo', 'clang_index_getObjCContainerDeclInfo', 'clang_index_getObjCInterfaceDeclInfo', 'clang_index_getObjCPropertyDeclInfo', 'clang_index_getObjCProtocolRefListInfo', 'clang_index_isEntityObjCContainerKind', 'clang_index_setClientContainer', 'clang_index_setClientEntity', 'clang_install_aborting_llvm_fatal_error_handler', 'clang_isAttribute', 'clang_isConstQualifiedType', 'clang_isCursorDefinition', 'clang_isDeclaration', 'clang_isExpression', 'clang_isFileMultipleIncludeGuarded', 'clang_isFunctionTypeVariadic', 'clang_isInvalid', 'clang_isInvalidDeclaration', 'clang_isPODType', 'clang_isPreprocessing', 'clang_isReference', 'clang_isRestrictQualifiedType', 'clang_isStatement', 'clang_isTranslationUnit', 'clang_isUnexposed', 'clang_isVirtualBase', 'clang_isVolatileQualifiedType', 'clang_loadDiagnostics', 'clang_parseTranslationUnit', 'clang_parseTranslationUnit2', 'clang_parseTranslationUnit2FullArgv', 'clang_remap_dispose', 'clang_remap_getFilenames', 'clang_remap_getNumFiles', 'clang_reparseTranslationUnit', 'clang_saveTranslationUnit', 'clang_sortCodeCompletionResults', 'clang_suspendTranslationUnit', 'clang_toggleCrashRecovery', 'clang_tokenize', 'clang_uninstall_llvm_fatal_error_handler', 'clang_visitChildren', 'constCXIdxAttrInfopconstp', 'constCXIdxBaseClassInfopconstp', 'constCXIdxObjCProtocolRefInfopconstp', 'constcharpconstp', 'constcharpp', 'constvoidp', 'voidp', 'voidpp']
+__all__ = ['CXAPISetImplp', 'CXAPISetImplpp', 'CXAvailabilityKind', 'CXBinaryOperatorKind', 'CXCallingConv', 'CXChildVisitResult', 'CXChoice', 'CXCodeCompleteResults', 'CXCodeComplete_Flags', 'CXComment', 'CXCommentInlineCommandRenderKind', 'CXCommentKind', 'CXCommentParamPassDirection', 'CXCompilationDatabase_Error', 'CXCompletionChunkKind', 'CXCompletionContext', 'CXCompletionResult', 'CXCursor', 'CXCursorAndRangeVisitor', 'CXCursorKind', 'CXCursorSetImplp', 'CXCursor_ExceptionSpecificationKind', 'CXCursorpp', 'CXDiagnosticDisplayOptions', 'CXDiagnosticSeverity', 'CXErrorCode', 'CXEvalResultKind', 'CXFileUniqueID', 'CXGlobalOptFlags', 'CXIdxAttrInfo', 'CXIdxAttrKind', 'CXIdxBaseClassInfo', 'CXIdxCXXClassDeclInfo', 'CXIdxContainerInfo', 'CXIdxDeclInfo', 'CXIdxDeclInfoFlags', 'CXIdxEntityCXXTemplateKind', 'CXIdxEntityInfo', 'CXIdxEntityKind', 'CXIdxEntityLanguage', 'CXIdxEntityRefInfo', 'CXIdxEntityRefKind', 'CXIdxIBOutletCollectionAttrInfo', 'CXIdxImportedASTFileInfo', 'CXIdxIncludedFileInfo', 'CXIdxLoc', 'CXIdxObjCCategoryDeclInfo', 'CXIdxObjCContainerDeclInfo', 'CXIdxObjCContainerKind', 'CXIdxObjCInterfaceDeclInfo', 'CXIdxObjCPropertyDeclInfo', 'CXIdxObjCProtocolRefInfo', 'CXIdxObjCProtocolRefListInfo', 'CXIndexOptFlags', 'CXIndexOptions', 'CXLanguageKind', 'CXLinkageKind', 'CXLoadDiag_Error', 'CXModuleMapDescriptorImplp', 'CXNameRefFlags', 'CXObjCDeclQualifierKind', 'CXObjCPropertyAttrKind', 'CXPlatformAvailability', 'CXPrintingPolicyProperty', 'CXRefQualifierKind', 'CXReparse_Flags', 'CXResult', 'CXSaveError', 'CXSaveTranslationUnit_Flags', 'CXSourceLocation', 'CXSourceRange', 'CXSourceRangeList', 'CXString', 'CXStringSet', 'CXSymbolRole', 'CXTLSKind', 'CXTUResourceUsage', 'CXTUResourceUsageEntry', 'CXTUResourceUsageKind', 'CXTargetInfoImplp', 'CXTemplateArgumentKind', 'CXToken', 'CXTokenKind', 'CXTokenpp', 'CXTranslationUnitImplp', 'CXTranslationUnitImplpp', 'CXTranslationUnit_Flags', 'CXType', 'CXTypeKind', 'CXTypeLayoutError', 'CXTypeNullabilityKind', 'CXUnaryOperatorKind', 'CXUnsavedFile', 'CXVersion', 'CXVirtualFileOverlayImplp', 'CXVisibilityKind', 'CXVisitorResult', 'CX_CXXAccessSpecifier', 'CX_StorageClass', 'IndexerCallbacks', 'StringHolder', 'TokenArray', 'charpp', 'clang_BlockCommandComment_getArgText', 'clang_BlockCommandComment_getCommandName', 'clang_BlockCommandComment_getNumArgs', 'clang_BlockCommandComment_getParagraph', 'clang_CXCursorSet_contains', 'clang_CXCursorSet_insert', 'clang_CXIndex_getGlobalOptions', 'clang_CXIndex_setGlobalOptions', 'clang_CXIndex_setInvocationEmissionPathOption', 'clang_CXRewriter_create', 'clang_CXRewriter_dispose', 'clang_CXRewriter_insertTextBefore', 'clang_CXRewriter_overwriteChangedFiles', 'clang_CXRewriter_removeText', 'clang_CXRewriter_replaceText', 'clang_CXRewriter_writeMainFileToStdOut', 'clang_CXXConstructor_isConvertingConstructor', 'clang_CXXConstructor_isCopyConstructor', 'clang_CXXConstructor_isDefaultConstructor', 'clang_CXXConstructor_isMoveConstructor', 'clang_CXXField_isMutable', 'clang_CXXMethod_isConst', 'clang_CXXMethod_isCopyAssignmentOperator', 'clang_CXXMethod_isDefaulted', 'clang_CXXMethod_isDeleted', 'clang_CXXMethod_isExplicit', 'clang_CXXMethod_isMoveAssignmentOperator', 'clang_CXXMethod_isPureVirtual', 'clang_CXXMethod_isStatic', 'clang_CXXMethod_isVirtual', 'clang_CXXRecord_isAbstract', 'clang_Comment_getChild', 'clang_Comment_getKind', 'clang_Comment_getNumChildren', 'clang_Comment_isWhitespace', 'clang_CompilationDatabase_dispose', 'clang_CompilationDatabase_fromDirectory', 'clang_CompilationDatabase_getAllCompileCommands', 'clang_CompilationDatabase_getCompileCommands', 'clang_CompileCommand_getArg', 'clang_CompileCommand_getDirectory', 'clang_CompileCommand_getFilename', 'clang_CompileCommand_getMappedSourceContent', 'clang_CompileCommand_getMappedSourcePath', 'clang_CompileCommand_getNumArgs', 'clang_CompileCommand_getNumMappedSources', 'clang_CompileCommands_dispose', 'clang_CompileCommands_getCommand', 'clang_CompileCommands_getSize', 'clang_Cursor_Evaluate', 'clang_Cursor_getArgument', 'clang_Cursor_getBriefCommentText', 'clang_Cursor_getCXXManglings', 'clang_Cursor_getCommentRange', 'clang_Cursor_getMangling', 'clang_Cursor_getModule', 'clang_Cursor_getNumArguments', 'clang_Cursor_getNumTemplateArguments', 'clang_Cursor_getObjCDeclQualifiers', 'clang_Cursor_getObjCManglings', 'clang_Cursor_getObjCPropertyAttributes', 'clang_Cursor_getObjCPropertyGetterName', 'clang_Cursor_getObjCPropertySetterName', 'clang_Cursor_getObjCSelectorIndex', 'clang_Cursor_getOffsetOfField', 'clang_Cursor_getParsedComment', 'clang_Cursor_getRawCommentText', 'clang_Cursor_getReceiverType', 'clang_Cursor_getSpellingNameRange', 'clang_Cursor_getStorageClass', 'clang_Cursor_getTemplateArgumentKind', 'clang_Cursor_getTemplateArgumentType', 'clang_Cursor_getTemplateArgumentUnsignedValue', 'clang_Cursor_getTemplateArgumentValue', 'clang_Cursor_getTranslationUnit', 'clang_Cursor_getVarDeclInitializer', 'clang_Cursor_hasAttrs', 'clang_Cursor_hasVarDeclExternalStorage', 'clang_Cursor_hasVarDeclGlobalStorage', 'clang_Cursor_isAnonymous', 'clang_Cursor_isAnonymousRecordDecl', 'clang_Cursor_isBitField', 'clang_Cursor_isDynamicCall', 'clang_Cursor_isExternalSymbol', 'clang_Cursor_isFunctionInlined', 'clang_Cursor_isInlineNamespace', 'clang_Cursor_isMacroBuiltin', 'clang_Cursor_isMacroFunctionLike', 'clang_Cursor_isNull', 'clang_Cursor_isObjCOptional', 'clang_Cursor_isVariadic', 'clang_EnumDecl_isScoped', 'clang_EvalResult_dispose', 'clang_EvalResult_getAsDouble', 'clang_EvalResult_getAsInt', 'clang_EvalResult_getAsLongLong', 'clang_EvalResult_getAsStr', 'clang_EvalResult_getAsUnsigned', 'clang_EvalResult_getKind', 'clang_EvalResult_isUnsignedInt', 'clang_File_isEqual', 'clang_File_tryGetRealPathName', 'clang_FullComment_getAsHTML', 'clang_FullComment_getAsXML', 'clang_HTMLStartTagComment_isSelfClosing', 'clang_HTMLStartTag_getAttrName', 'clang_HTMLStartTag_getAttrValue', 'clang_HTMLStartTag_getNumAttrs', 'clang_HTMLTagComment_getAsString', 'clang_HTMLTagComment_getTagName', 'clang_IndexAction_create', 'clang_IndexAction_dispose', 'clang_InlineCommandComment_getArgText', 'clang_InlineCommandComment_getCommandName', 'clang_InlineCommandComment_getNumArgs', 'clang_InlineCommandComment_getRenderKind', 'clang_InlineContentComment_hasTrailingNewline', 'clang_Location_isFromMainFile', 'clang_Location_isInSystemHeader', 'clang_ModuleMapDescriptor_create', 'clang_ModuleMapDescriptor_dispose', 'clang_ModuleMapDescriptor_setFrameworkModuleName', 'clang_ModuleMapDescriptor_setUmbrellaHeader', 'clang_ModuleMapDescriptor_writeToBuffer', 'clang_Module_getASTFile', 'clang_Module_getFullName', 'clang_Module_getName', 'clang_Module_getNumTopLevelHeaders', 'clang_Module_getParent', 'clang_Module_getTopLevelHeader', 'clang_Module_isSystem', 'clang_ParamCommandComment_getDirection', 'clang_ParamCommandComment_getParamIndex', 'clang_ParamCommandComment_getParamName', 'clang_ParamCommandComment_isDirectionExplicit', 'clang_ParamCommandComment_isParamIndexValid', 'clang_PrintingPolicy_dispose', 'clang_PrintingPolicy_getProperty', 'clang_PrintingPolicy_setProperty', 'clang_Range_isNull', 'clang_TParamCommandComment_getDepth', 'clang_TParamCommandComment_getIndex', 'clang_TParamCommandComment_getParamName', 'clang_TParamCommandComment_isParamPositionValid', 'clang_TargetInfo_dispose', 'clang_TargetInfo_getPointerWidth', 'clang_TargetInfo_getTriple', 'clang_TextComment_getText', 'clang_Type_getAlignOf', 'clang_Type_getCXXRefQualifier', 'clang_Type_getClassType', 'clang_Type_getModifiedType', 'clang_Type_getNamedType', 'clang_Type_getNullability', 'clang_Type_getNumObjCProtocolRefs', 'clang_Type_getNumObjCTypeArgs', 'clang_Type_getNumTemplateArguments', 'clang_Type_getObjCEncoding', 'clang_Type_getObjCObjectBaseType', 'clang_Type_getObjCProtocolDecl', 'clang_Type_getObjCTypeArg', 'clang_Type_getOffsetOf', 'clang_Type_getSizeOf', 'clang_Type_getTemplateArgumentAsType', 'clang_Type_getValueType', 'clang_Type_isTransparentTagTypedef', 'clang_Type_visitFields', 'clang_VerbatimBlockLineComment_getText', 'clang_VerbatimLineComment_getText', 'clang_VirtualFileOverlay_addFileMapping', 'clang_VirtualFileOverlay_create', 'clang_VirtualFileOverlay_dispose', 'clang_VirtualFileOverlay_setCaseSensitivity', 'clang_VirtualFileOverlay_writeToBuffer', 'clang_annotateTokens', 'clang_codeCompleteAt', 'clang_codeCompleteGetContainerKind', 'clang_codeCompleteGetContainerUSR', 'clang_codeCompleteGetContexts', 'clang_codeCompleteGetDiagnostic', 'clang_codeCompleteGetNumDiagnostics', 'clang_codeCompleteGetObjCSelector', 'clang_constructUSR_ObjCCategory', 'clang_constructUSR_ObjCClass', 'clang_constructUSR_ObjCIvar', 'clang_constructUSR_ObjCMethod', 'clang_constructUSR_ObjCProperty', 'clang_constructUSR_ObjCProtocol', 'clang_createAPISet', 'clang_createCXCursorSet', 'clang_createIndex', 'clang_createIndexWithOptions', 'clang_createTranslationUnit', 'clang_createTranslationUnit2', 'clang_createTranslationUnitFromSourceFile', 'clang_defaultCodeCompleteOptions', 'clang_defaultDiagnosticDisplayOptions', 'clang_defaultEditingTranslationUnitOptions', 'clang_defaultReparseOptions', 'clang_defaultSaveOptions', 'clang_disposeAPISet', 'clang_disposeCXCursorSet', 'clang_disposeCXPlatformAvailability', 'clang_disposeCXTUResourceUsage', 'clang_disposeCodeCompleteResults', 'clang_disposeDiagnostic', 'clang_disposeDiagnosticSet', 'clang_disposeIndex', 'clang_disposeOverriddenCursors', 'clang_disposeSourceRangeList', 'clang_disposeString', 'clang_disposeStringSet', 'clang_disposeTokens', 'clang_disposeTranslationUnit', 'clang_enableStackTraces', 'clang_equalCursors', 'clang_equalLocations', 'clang_equalRanges', 'clang_equalTypes', 'clang_executeOnThread', 'clang_findIncludesInFile', 'clang_findIncludesInFileWithBlock', 'clang_findReferencesInFile', 'clang_findReferencesInFileWithBlock', 'clang_formatDiagnostic', 'clang_free', 'clang_getAddressSpace', 'clang_getAllSkippedRanges', 'clang_getArgType', 'clang_getArrayElementType', 'clang_getArraySize', 'clang_getBinaryOperatorKindSpelling', 'clang_getBuildSessionTimestamp', 'clang_getCString', 'clang_getCXTUResourceUsage', 'clang_getCXXAccessSpecifier', 'clang_getCanonicalCursor', 'clang_getCanonicalType', 'clang_getChildDiagnostics', 'clang_getClangVersion', 'clang_getCompletionAnnotation', 'clang_getCompletionAvailability', 'clang_getCompletionBriefComment', 'clang_getCompletionChunkCompletionString', 'clang_getCompletionChunkKind', 'clang_getCompletionChunkText', 'clang_getCompletionFixIt', 'clang_getCompletionNumAnnotations', 'clang_getCompletionNumFixIts', 'clang_getCompletionParent', 'clang_getCompletionPriority', 'clang_getCursor', 'clang_getCursorAvailability', 'clang_getCursorBinaryOperatorKind', 'clang_getCursorCompletionString', 'clang_getCursorDefinition', 'clang_getCursorDisplayName', 'clang_getCursorExceptionSpecificationType', 'clang_getCursorExtent', 'clang_getCursorKind', 'clang_getCursorKindSpelling', 'clang_getCursorLanguage', 'clang_getCursorLexicalParent', 'clang_getCursorLinkage', 'clang_getCursorLocation', 'clang_getCursorPlatformAvailability', 'clang_getCursorPrettyPrinted', 'clang_getCursorPrintingPolicy', 'clang_getCursorReferenceNameRange', 'clang_getCursorReferenced', 'clang_getCursorResultType', 'clang_getCursorSemanticParent', 'clang_getCursorSpelling', 'clang_getCursorTLSKind', 'clang_getCursorType', 'clang_getCursorUSR', 'clang_getCursorUnaryOperatorKind', 'clang_getCursorVisibility', 'clang_getDeclObjCTypeEncoding', 'clang_getDefinitionSpellingAndExtent', 'clang_getDiagnostic', 'clang_getDiagnosticCategory', 'clang_getDiagnosticCategoryName', 'clang_getDiagnosticCategoryText', 'clang_getDiagnosticFixIt', 'clang_getDiagnosticInSet', 'clang_getDiagnosticLocation', 'clang_getDiagnosticNumFixIts', 'clang_getDiagnosticNumRanges', 'clang_getDiagnosticOption', 'clang_getDiagnosticRange', 'clang_getDiagnosticSetFromTU', 'clang_getDiagnosticSeverity', 'clang_getDiagnosticSpelling', 'clang_getElementType', 'clang_getEnumConstantDeclUnsignedValue', 'clang_getEnumConstantDeclValue', 'clang_getEnumDeclIntegerType', 'clang_getExceptionSpecificationType', 'clang_getExpansionLocation', 'clang_getFieldDeclBitWidth', 'clang_getFile', 'clang_getFileContents', 'clang_getFileLocation', 'clang_getFileName', 'clang_getFileTime', 'clang_getFileUniqueID', 'clang_getFunctionTypeCallingConv', 'clang_getIBOutletCollectionType', 'clang_getIncludedFile', 'clang_getInclusions', 'clang_getInstantiationLocation', 'clang_getLocation', 'clang_getLocationForOffset', 'clang_getModuleForFile', 'clang_getNonReferenceType', 'clang_getNullCursor', 'clang_getNullLocation', 'clang_getNullRange', 'clang_getNumArgTypes', 'clang_getNumCompletionChunks', 'clang_getNumDiagnostics', 'clang_getNumDiagnosticsInSet', 'clang_getNumElements', 'clang_getNumOverloadedDecls', 'clang_getOverloadedDecl', 'clang_getOverriddenCursors', 'clang_getPointeeType', 'clang_getPresumedLocation', 'clang_getRange', 'clang_getRangeEnd', 'clang_getRangeStart', 'clang_getRemappings', 'clang_getRemappingsFromFileList', 'clang_getResultType', 'clang_getSkippedRanges', 'clang_getSpecializedCursorTemplate', 'clang_getSpellingLocation', 'clang_getSymbolGraphForCursor', 'clang_getSymbolGraphForUSR', 'clang_getTUResourceUsageName', 'clang_getTemplateCursorKind', 'clang_getToken', 'clang_getTokenExtent', 'clang_getTokenKind', 'clang_getTokenLocation', 'clang_getTokenSpelling', 'clang_getTranslationUnitCursor', 'clang_getTranslationUnitSpelling', 'clang_getTranslationUnitTargetInfo', 'clang_getTypeDeclaration', 'clang_getTypeKindSpelling', 'clang_getTypeSpelling', 'clang_getTypedefDeclUnderlyingType', 'clang_getTypedefName', 'clang_getUnaryOperatorKindSpelling', 'clang_getUnqualifiedType', 'clang_hashCursor', 'clang_indexLoc_getCXSourceLocation', 'clang_indexLoc_getFileLocation', 'clang_indexSourceFile', 'clang_indexSourceFileFullArgv', 'clang_indexTranslationUnit', 'clang_index_getCXXClassDeclInfo', 'clang_index_getClientContainer', 'clang_index_getClientEntity', 'clang_index_getIBOutletCollectionAttrInfo', 'clang_index_getObjCCategoryDeclInfo', 'clang_index_getObjCContainerDeclInfo', 'clang_index_getObjCInterfaceDeclInfo', 'clang_index_getObjCPropertyDeclInfo', 'clang_index_getObjCProtocolRefListInfo', 'clang_index_isEntityObjCContainerKind', 'clang_index_setClientContainer', 'clang_index_setClientEntity', 'clang_install_aborting_llvm_fatal_error_handler', 'clang_isAttribute', 'clang_isConstQualifiedType', 'clang_isCursorDefinition', 'clang_isDeclaration', 'clang_isExpression', 'clang_isFileMultipleIncludeGuarded', 'clang_isFunctionTypeVariadic', 'clang_isInvalid', 'clang_isInvalidDeclaration', 'clang_isPODType', 'clang_isPreprocessing', 'clang_isReference', 'clang_isRestrictQualifiedType', 'clang_isStatement', 'clang_isTranslationUnit', 'clang_isUnexposed', 'clang_isVirtualBase', 'clang_isVolatileQualifiedType', 'clang_loadDiagnostics', 'clang_parseTranslationUnit', 'clang_parseTranslationUnit2', 'clang_parseTranslationUnit2FullArgv', 'clang_remap_dispose', 'clang_remap_getFilenames', 'clang_remap_getNumFiles', 'clang_reparseTranslationUnit', 'clang_saveTranslationUnit', 'clang_sortCodeCompletionResults', 'clang_suspendTranslationUnit', 'clang_toggleCrashRecovery', 'clang_tokenize', 'clang_uninstall_llvm_fatal_error_handler', 'clang_visitChildren', 'clang_visitChildrenWithBlock', 'constCXIdxAttrInfopconstp', 'constCXIdxBaseClassInfopconstp', 'constCXIdxObjCProtocolRefInfopconstp', 'constcharpconstp', 'constcharpp', 'constvoidp', 'voidp', 'voidpp']
 class CXAPISetImplp(_PointerWrapperBase):
     @staticmethod
     def from_capsule(arg0: capsule) -> CXAPISetImplp:
         ...
     def __init__(self, arg0: int) -> None:
         ...
 class CXAPISetImplpp(_PointerWrapperBase):
@@ -90,14 +90,173 @@
         ...
     @property
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
+class CXBinaryOperatorKind:
+    """
+    /**
+     * Describes the kind of binary operators.
+     */
+    
+    Members:
+    
+      CXBinaryOperator_Invalid : /** This value describes cursors which are not binary operators. */
+    
+      CXBinaryOperator_PtrMemD : /** C++ Pointer - to - member operator. */
+    
+      CXBinaryOperator_PtrMemI : /** C++ Pointer - to - member operator. */
+    
+      CXBinaryOperator_Mul : /** Multiplication operator. */
+    
+      CXBinaryOperator_Div : /** Division operator. */
+    
+      CXBinaryOperator_Rem : /** Remainder operator. */
+    
+      CXBinaryOperator_Add : /** Addition operator. */
+    
+      CXBinaryOperator_Sub : /** Subtraction operator. */
+    
+      CXBinaryOperator_Shl : /** Bitwise shift left operator. */
+    
+      CXBinaryOperator_Shr : /** Bitwise shift right operator. */
+    
+      CXBinaryOperator_Cmp : /** C++ three-way comparison (spaceship) operator. */
+    
+      CXBinaryOperator_LT : /** Less than operator. */
+    
+      CXBinaryOperator_GT : /** Greater than operator. */
+    
+      CXBinaryOperator_LE : /** Less or equal operator. */
+    
+      CXBinaryOperator_GE : /** Greater or equal operator. */
+    
+      CXBinaryOperator_EQ : /** Equal operator. */
+    
+      CXBinaryOperator_NE : /** Not equal operator. */
+    
+      CXBinaryOperator_And : /** Bitwise AND operator. */
+    
+      CXBinaryOperator_Xor : /** Bitwise XOR operator. */
+    
+      CXBinaryOperator_Or : /** Bitwise OR operator. */
+    
+      CXBinaryOperator_LAnd : /** Logical AND operator. */
+    
+      CXBinaryOperator_LOr : /** Logical OR operator. */
+    
+      CXBinaryOperator_Assign : /** Assignment operator. */
+    
+      CXBinaryOperator_MulAssign : /** Multiplication assignment operator. */
+    
+      CXBinaryOperator_DivAssign : /** Division assignment operator. */
+    
+      CXBinaryOperator_RemAssign : /** Remainder assignment operator. */
+    
+      CXBinaryOperator_AddAssign : /** Addition assignment operator. */
+    
+      CXBinaryOperator_SubAssign : /** Subtraction assignment operator. */
+    
+      CXBinaryOperator_ShlAssign : /** Bitwise shift left assignment operator. */
+    
+      CXBinaryOperator_ShrAssign : /** Bitwise shift right assignment operator. */
+    
+      CXBinaryOperator_AndAssign : /** Bitwise AND assignment operator. */
+    
+      CXBinaryOperator_XorAssign : /** Bitwise XOR assignment operator. */
+    
+      CXBinaryOperator_OrAssign : /** Bitwise OR assignment operator. */
+    
+      CXBinaryOperator_Comma : /** Comma operator. */
+    """
+    CXBinaryOperator_Add: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Add: 6>
+    CXBinaryOperator_AddAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_AddAssign: 26>
+    CXBinaryOperator_And: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_And: 17>
+    CXBinaryOperator_AndAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_AndAssign: 30>
+    CXBinaryOperator_Assign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Assign: 22>
+    CXBinaryOperator_Cmp: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Cmp: 10>
+    CXBinaryOperator_Comma: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Comma: 33>
+    CXBinaryOperator_Div: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Div: 4>
+    CXBinaryOperator_DivAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_DivAssign: 24>
+    CXBinaryOperator_EQ: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_EQ: 15>
+    CXBinaryOperator_GE: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_GE: 14>
+    CXBinaryOperator_GT: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_GT: 12>
+    CXBinaryOperator_Invalid: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Invalid: 0>
+    CXBinaryOperator_LAnd: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_LAnd: 20>
+    CXBinaryOperator_LE: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_LE: 13>
+    CXBinaryOperator_LOr: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_LOr: 21>
+    CXBinaryOperator_LT: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_LT: 11>
+    CXBinaryOperator_Mul: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Mul: 3>
+    CXBinaryOperator_MulAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_MulAssign: 23>
+    CXBinaryOperator_NE: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_NE: 16>
+    CXBinaryOperator_Or: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Or: 19>
+    CXBinaryOperator_OrAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_OrAssign: 32>
+    CXBinaryOperator_PtrMemD: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_PtrMemD: 1>
+    CXBinaryOperator_PtrMemI: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_PtrMemI: 2>
+    CXBinaryOperator_Rem: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Rem: 5>
+    CXBinaryOperator_RemAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_RemAssign: 25>
+    CXBinaryOperator_Shl: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Shl: 8>
+    CXBinaryOperator_ShlAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_ShlAssign: 28>
+    CXBinaryOperator_Shr: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Shr: 9>
+    CXBinaryOperator_ShrAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_ShrAssign: 29>
+    CXBinaryOperator_Sub: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Sub: 7>
+    CXBinaryOperator_SubAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_SubAssign: 27>
+    CXBinaryOperator_Xor: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_Xor: 18>
+    CXBinaryOperator_XorAssign: typing.ClassVar[CXBinaryOperatorKind]  # value = <CXBinaryOperatorKind.CXBinaryOperator_XorAssign: 31>
+    __members__: typing.ClassVar[dict[str, CXBinaryOperatorKind]]  # value = {'CXBinaryOperator_Invalid': <CXBinaryOperatorKind.CXBinaryOperator_Invalid: 0>, 'CXBinaryOperator_PtrMemD': <CXBinaryOperatorKind.CXBinaryOperator_PtrMemD: 1>, 'CXBinaryOperator_PtrMemI': <CXBinaryOperatorKind.CXBinaryOperator_PtrMemI: 2>, 'CXBinaryOperator_Mul': <CXBinaryOperatorKind.CXBinaryOperator_Mul: 3>, 'CXBinaryOperator_Div': <CXBinaryOperatorKind.CXBinaryOperator_Div: 4>, 'CXBinaryOperator_Rem': <CXBinaryOperatorKind.CXBinaryOperator_Rem: 5>, 'CXBinaryOperator_Add': <CXBinaryOperatorKind.CXBinaryOperator_Add: 6>, 'CXBinaryOperator_Sub': <CXBinaryOperatorKind.CXBinaryOperator_Sub: 7>, 'CXBinaryOperator_Shl': <CXBinaryOperatorKind.CXBinaryOperator_Shl: 8>, 'CXBinaryOperator_Shr': <CXBinaryOperatorKind.CXBinaryOperator_Shr: 9>, 'CXBinaryOperator_Cmp': <CXBinaryOperatorKind.CXBinaryOperator_Cmp: 10>, 'CXBinaryOperator_LT': <CXBinaryOperatorKind.CXBinaryOperator_LT: 11>, 'CXBinaryOperator_GT': <CXBinaryOperatorKind.CXBinaryOperator_GT: 12>, 'CXBinaryOperator_LE': <CXBinaryOperatorKind.CXBinaryOperator_LE: 13>, 'CXBinaryOperator_GE': <CXBinaryOperatorKind.CXBinaryOperator_GE: 14>, 'CXBinaryOperator_EQ': <CXBinaryOperatorKind.CXBinaryOperator_EQ: 15>, 'CXBinaryOperator_NE': <CXBinaryOperatorKind.CXBinaryOperator_NE: 16>, 'CXBinaryOperator_And': <CXBinaryOperatorKind.CXBinaryOperator_And: 17>, 'CXBinaryOperator_Xor': <CXBinaryOperatorKind.CXBinaryOperator_Xor: 18>, 'CXBinaryOperator_Or': <CXBinaryOperatorKind.CXBinaryOperator_Or: 19>, 'CXBinaryOperator_LAnd': <CXBinaryOperatorKind.CXBinaryOperator_LAnd: 20>, 'CXBinaryOperator_LOr': <CXBinaryOperatorKind.CXBinaryOperator_LOr: 21>, 'CXBinaryOperator_Assign': <CXBinaryOperatorKind.CXBinaryOperator_Assign: 22>, 'CXBinaryOperator_MulAssign': <CXBinaryOperatorKind.CXBinaryOperator_MulAssign: 23>, 'CXBinaryOperator_DivAssign': <CXBinaryOperatorKind.CXBinaryOperator_DivAssign: 24>, 'CXBinaryOperator_RemAssign': <CXBinaryOperatorKind.CXBinaryOperator_RemAssign: 25>, 'CXBinaryOperator_AddAssign': <CXBinaryOperatorKind.CXBinaryOperator_AddAssign: 26>, 'CXBinaryOperator_SubAssign': <CXBinaryOperatorKind.CXBinaryOperator_SubAssign: 27>, 'CXBinaryOperator_ShlAssign': <CXBinaryOperatorKind.CXBinaryOperator_ShlAssign: 28>, 'CXBinaryOperator_ShrAssign': <CXBinaryOperatorKind.CXBinaryOperator_ShrAssign: 29>, 'CXBinaryOperator_AndAssign': <CXBinaryOperatorKind.CXBinaryOperator_AndAssign: 30>, 'CXBinaryOperator_XorAssign': <CXBinaryOperatorKind.CXBinaryOperator_XorAssign: 31>, 'CXBinaryOperator_OrAssign': <CXBinaryOperatorKind.CXBinaryOperator_OrAssign: 32>, 'CXBinaryOperator_Comma': <CXBinaryOperatorKind.CXBinaryOperator_Comma: 33>}
+    def __and__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __ge__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __gt__(self, other: typing.Any) -> bool:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __invert__(self) -> typing.Any:
+        ...
+    def __le__(self, other: typing.Any) -> bool:
+        ...
+    def __lt__(self, other: typing.Any) -> bool:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __or__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rand__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __ror__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rxor__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
+    def __xor__(self, other: typing.Any) -> typing.Any:
+        ...
+    @property
+    def name(self) -> str:
+        ...
+    @property
+    def value(self) -> int:
+        ...
 class CXCallingConv:
     """
     /**
      * Describes the calling convention of a function type
      */
     
     Members:
@@ -138,41 +297,44 @@
     
       CXCallingConv_AArch64VectorCall : /* Alias for compatibility with older versions of API. */
     
       CXCallingConv_SwiftAsync : /* Alias for compatibility with older versions of API. */
     
       CXCallingConv_AArch64SVEPCS : /* Alias for compatibility with older versions of API. */
     
+      CXCallingConv_M68kRTD : /* Alias for compatibility with older versions of API. */
+    
       CXCallingConv_Invalid : /* Alias for compatibility with older versions of API. */
     
       CXCallingConv_Unexposed : /* Alias for compatibility with older versions of API. */
     """
     CXCallingConv_AAPCS: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_AAPCS: 6>
     CXCallingConv_AAPCS_VFP: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_AAPCS_VFP: 7>
     CXCallingConv_AArch64SVEPCS: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_AArch64SVEPCS: 18>
     CXCallingConv_AArch64VectorCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_AArch64VectorCall: 16>
     CXCallingConv_C: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_C: 1>
     CXCallingConv_Default: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Default: 0>
     CXCallingConv_IntelOclBicc: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_IntelOclBicc: 9>
     CXCallingConv_Invalid: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Invalid: 100>
+    CXCallingConv_M68kRTD: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_M68kRTD: 19>
     CXCallingConv_PreserveAll: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_PreserveAll: 15>
     CXCallingConv_PreserveMost: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_PreserveMost: 14>
     CXCallingConv_Swift: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Swift: 13>
     CXCallingConv_SwiftAsync: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_SwiftAsync: 17>
     CXCallingConv_Unexposed: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Unexposed: 200>
     CXCallingConv_Win64: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Win64: 10>
     CXCallingConv_X86FastCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86FastCall: 3>
     CXCallingConv_X86Pascal: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86Pascal: 5>
     CXCallingConv_X86RegCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86RegCall: 8>
     CXCallingConv_X86StdCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86StdCall: 2>
     CXCallingConv_X86ThisCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86ThisCall: 4>
     CXCallingConv_X86VectorCall: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86VectorCall: 12>
     CXCallingConv_X86_64SysV: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_X86_64SysV: 11>
     CXCallingConv_X86_64Win64: typing.ClassVar[CXCallingConv]  # value = <CXCallingConv.CXCallingConv_Win64: 10>
-    __members__: typing.ClassVar[dict[str, CXCallingConv]]  # value = {'CXCallingConv_Default': <CXCallingConv.CXCallingConv_Default: 0>, 'CXCallingConv_C': <CXCallingConv.CXCallingConv_C: 1>, 'CXCallingConv_X86StdCall': <CXCallingConv.CXCallingConv_X86StdCall: 2>, 'CXCallingConv_X86FastCall': <CXCallingConv.CXCallingConv_X86FastCall: 3>, 'CXCallingConv_X86ThisCall': <CXCallingConv.CXCallingConv_X86ThisCall: 4>, 'CXCallingConv_X86Pascal': <CXCallingConv.CXCallingConv_X86Pascal: 5>, 'CXCallingConv_AAPCS': <CXCallingConv.CXCallingConv_AAPCS: 6>, 'CXCallingConv_AAPCS_VFP': <CXCallingConv.CXCallingConv_AAPCS_VFP: 7>, 'CXCallingConv_X86RegCall': <CXCallingConv.CXCallingConv_X86RegCall: 8>, 'CXCallingConv_IntelOclBicc': <CXCallingConv.CXCallingConv_IntelOclBicc: 9>, 'CXCallingConv_Win64': <CXCallingConv.CXCallingConv_Win64: 10>, 'CXCallingConv_X86_64Win64': <CXCallingConv.CXCallingConv_Win64: 10>, 'CXCallingConv_X86_64SysV': <CXCallingConv.CXCallingConv_X86_64SysV: 11>, 'CXCallingConv_X86VectorCall': <CXCallingConv.CXCallingConv_X86VectorCall: 12>, 'CXCallingConv_Swift': <CXCallingConv.CXCallingConv_Swift: 13>, 'CXCallingConv_PreserveMost': <CXCallingConv.CXCallingConv_PreserveMost: 14>, 'CXCallingConv_PreserveAll': <CXCallingConv.CXCallingConv_PreserveAll: 15>, 'CXCallingConv_AArch64VectorCall': <CXCallingConv.CXCallingConv_AArch64VectorCall: 16>, 'CXCallingConv_SwiftAsync': <CXCallingConv.CXCallingConv_SwiftAsync: 17>, 'CXCallingConv_AArch64SVEPCS': <CXCallingConv.CXCallingConv_AArch64SVEPCS: 18>, 'CXCallingConv_Invalid': <CXCallingConv.CXCallingConv_Invalid: 100>, 'CXCallingConv_Unexposed': <CXCallingConv.CXCallingConv_Unexposed: 200>}
+    __members__: typing.ClassVar[dict[str, CXCallingConv]]  # value = {'CXCallingConv_Default': <CXCallingConv.CXCallingConv_Default: 0>, 'CXCallingConv_C': <CXCallingConv.CXCallingConv_C: 1>, 'CXCallingConv_X86StdCall': <CXCallingConv.CXCallingConv_X86StdCall: 2>, 'CXCallingConv_X86FastCall': <CXCallingConv.CXCallingConv_X86FastCall: 3>, 'CXCallingConv_X86ThisCall': <CXCallingConv.CXCallingConv_X86ThisCall: 4>, 'CXCallingConv_X86Pascal': <CXCallingConv.CXCallingConv_X86Pascal: 5>, 'CXCallingConv_AAPCS': <CXCallingConv.CXCallingConv_AAPCS: 6>, 'CXCallingConv_AAPCS_VFP': <CXCallingConv.CXCallingConv_AAPCS_VFP: 7>, 'CXCallingConv_X86RegCall': <CXCallingConv.CXCallingConv_X86RegCall: 8>, 'CXCallingConv_IntelOclBicc': <CXCallingConv.CXCallingConv_IntelOclBicc: 9>, 'CXCallingConv_Win64': <CXCallingConv.CXCallingConv_Win64: 10>, 'CXCallingConv_X86_64Win64': <CXCallingConv.CXCallingConv_Win64: 10>, 'CXCallingConv_X86_64SysV': <CXCallingConv.CXCallingConv_X86_64SysV: 11>, 'CXCallingConv_X86VectorCall': <CXCallingConv.CXCallingConv_X86VectorCall: 12>, 'CXCallingConv_Swift': <CXCallingConv.CXCallingConv_Swift: 13>, 'CXCallingConv_PreserveMost': <CXCallingConv.CXCallingConv_PreserveMost: 14>, 'CXCallingConv_PreserveAll': <CXCallingConv.CXCallingConv_PreserveAll: 15>, 'CXCallingConv_AArch64VectorCall': <CXCallingConv.CXCallingConv_AArch64VectorCall: 16>, 'CXCallingConv_SwiftAsync': <CXCallingConv.CXCallingConv_SwiftAsync: 17>, 'CXCallingConv_AArch64SVEPCS': <CXCallingConv.CXCallingConv_AArch64SVEPCS: 18>, 'CXCallingConv_M68kRTD': <CXCallingConv.CXCallingConv_M68kRTD: 19>, 'CXCallingConv_Invalid': <CXCallingConv.CXCallingConv_Invalid: 100>, 'CXCallingConv_Unexposed': <CXCallingConv.CXCallingConv_Unexposed: 200>}
     def __and__(self, other: typing.Any) -> typing.Any:
         ...
     def __eq__(self, other: typing.Any) -> bool:
         ...
     def __ge__(self, other: typing.Any) -> bool:
         ...
     def __getstate__(self) -> int:
@@ -220,15 +382,15 @@
 class CXChildVisitResult:
     """
     /**
      * Describes how the traversal of the children of a particular
      * cursor should proceed after visiting a particular child cursor.
      *
      * A value of this enumeration type should be returned by each
-     * \c CXCursorVisitor to indicate how clang_visitChildren() proceed.
+     * \\c CXCursorVisitor to indicate how clang_visitChildren() proceed.
      */
     
     Members:
     
       CXChildVisit_Break : /**
        * Terminates the cursor traversal.
        */
@@ -291,47 +453,116 @@
         ...
     @property
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
+class CXChoice:
+    """
+    Members:
+    
+      CXChoice_Default : /**
+       * Use the default value of an option that may depend on the process
+       * environment.
+       */
+    
+      CXChoice_Enabled : /**
+       * Enable the option.
+       */
+    
+      CXChoice_Disabled : /**
+       * Disable the option.
+       */
+    """
+    CXChoice_Default: typing.ClassVar[CXChoice]  # value = <CXChoice.CXChoice_Default: 0>
+    CXChoice_Disabled: typing.ClassVar[CXChoice]  # value = <CXChoice.CXChoice_Disabled: 2>
+    CXChoice_Enabled: typing.ClassVar[CXChoice]  # value = <CXChoice.CXChoice_Enabled: 1>
+    __members__: typing.ClassVar[dict[str, CXChoice]]  # value = {'CXChoice_Default': <CXChoice.CXChoice_Default: 0>, 'CXChoice_Enabled': <CXChoice.CXChoice_Enabled: 1>, 'CXChoice_Disabled': <CXChoice.CXChoice_Disabled: 2>}
+    def __and__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __ge__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __gt__(self, other: typing.Any) -> bool:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __invert__(self) -> typing.Any:
+        ...
+    def __le__(self, other: typing.Any) -> bool:
+        ...
+    def __lt__(self, other: typing.Any) -> bool:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __or__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rand__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __ror__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rxor__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
+    def __xor__(self, other: typing.Any) -> typing.Any:
+        ...
+    @property
+    def name(self) -> str:
+        ...
+    @property
+    def value(self) -> int:
+        ...
 class CXCodeCompleteResults:
     """
     /**
      * Contains the results of code-completion.
      *
      * This data structure contains the results of code completion, as
-     * produced by \c clang_codeCompleteAt(). Its contents must be freed by
-     * \c clang_disposeCodeCompleteResults.
+     * produced by \\c clang_codeCompleteAt(). Its contents must be freed by
+     * \\c clang_disposeCodeCompleteResults.
      */
     """
     def __init__(self) -> None:
         ...
     def at(self, arg0: int) -> CXCompletionResult:
         ...
     @property
     def NumResults(self) -> int:
         """
         /**
            * The number of code-completion results stored in the
-           * \c Results array.
+           * \\c Results array.
            */
         """
     @NumResults.setter
     def NumResults(self, arg0: int) -> None:
         ...
 class CXCodeComplete_Flags:
     """
     /**
-     * Flags that can be passed to \c clang_codeCompleteAt() to
+     * Flags that can be passed to \\c clang_codeCompleteAt() to
      * modify its behavior.
      *
      * The enumerators in this enumeration can be bitwise-OR'd together to
-     * provide multiple options to \c clang_codeCompleteAt().
+     * provide multiple options to \\c clang_codeCompleteAt().
      */
     
     Members:
     
       CXCodeComplete_IncludeMacros : /**
        * Whether to include macros within the set of code
        * completions returned.
@@ -503,15 +734,15 @@
         ...
     @property
     def value(self) -> int:
         ...
 class CXCommentKind:
     """
     /**
-     * Describes the type of the comment AST node (\c CXComment).  A comment
+     * Describes the type of the comment AST node (\\c CXComment).  A comment
      * node can be considered block content (e. g., paragraph), inline content
      * (plain text) or neither (the root AST node).
      */
     
     Members:
     
       CXComment_Null : /**
@@ -522,77 +753,77 @@
       CXComment_Text : /**
        * Plain text.  Inline content.
        */
     
       CXComment_InlineCommand : /**
        * A command with word-like arguments that is considered inline content.
        *
-       * For example: \\c command.
+       * For example: \\\\c command.
        */
     
       CXComment_HTMLStartTag : /**
        * HTML start tag with attributes (name-value pairs).  Considered
        * inline content.
        *
        * For example:
-       * \verbatim
+       * \\verbatim
        * <br> <br /> <a href="http://example.org/">
-       * \endverbatim
+       * \\endverbatim
        */
     
       CXComment_HTMLEndTag : /**
        * HTML end tag.  Considered inline content.
        *
        * For example:
-       * \verbatim
+       * \\verbatim
        * </a>
-       * \endverbatim
+       * \\endverbatim
        */
     
       CXComment_Paragraph : /**
        * A paragraph, contains inline comment.  The paragraph itself is
        * block content.
        */
     
       CXComment_BlockCommand : /**
        * A command that has zero or more word-like arguments (number of
        * word-like arguments depends on command name) and a paragraph as an
        * argument.  Block command is block content.
        *
        * Paragraph argument is also a child of the block command.
        *
-       * For example: \has 0 word-like arguments and a paragraph argument.
+       * For example: \\has 0 word-like arguments and a paragraph argument.
        *
-       * AST nodes of special kinds that parser knows about (e. g., \\param
+       * AST nodes of special kinds that parser knows about (e. g., \\\\param
        * command) have their own node kinds.
        */
     
       CXComment_ParamCommand : /**
-       * A \\param or \\arg command that describes the function parameter
+       * A \\\\param or \\\\arg command that describes the function parameter
        * (name, passing direction, description).
        *
-       * For example: \\param [in] ParamName description.
+       * For example: \\\\param [in] ParamName description.
        */
     
       CXComment_TParamCommand : /**
-       * A \\tparam command that describes a template parameter (name and
+       * A \\\\tparam command that describes a template parameter (name and
        * description).
        *
-       * For example: \\tparam T description.
+       * For example: \\\\tparam T description.
        */
     
       CXComment_VerbatimBlockCommand : /**
        * A verbatim block command (e. g., preformatted code).  Verbatim
        * block has an opening and a closing command and contains multiple lines of
-       * text (\c CXComment_VerbatimBlockLine child nodes).
+       * text (\\c CXComment_VerbatimBlockLine child nodes).
        *
        * For example:
-       * \\verbatim
+       * \\\\verbatim
        * aaa
-       * \\endverbatim
+       * \\\\endverbatim
        */
     
       CXComment_VerbatimBlockLine : /**
        * A line of text that is contained within a
        * CXComment_VerbatimBlockCommand node.
        */
     
@@ -667,15 +898,15 @@
         ...
     @property
     def value(self) -> int:
         ...
 class CXCommentParamPassDirection:
     """
     /**
-     * Describes parameter passing direction for \\param or \\arg command.
+     * Describes parameter passing direction for \\\\param or \\\\arg command.
      */
     
     Members:
     
       CXCommentParamPassDirection_In : /**
        * The parameter is an input parameter.
        */
@@ -808,35 +1039,35 @@
     def value(self) -> int:
         ...
 class CXCompletionChunkKind:
     """
     /**
      * Describes a single piece of text within a code-completion string.
      *
-     * Each "chunk" within a code-completion string (\c CXCompletionString) is
+     * Each "chunk" within a code-completion string (\\c CXCompletionString) is
      * either a piece of text with a specific "kind" that describes how that text
      * should be interpreted by the client or is another completion string.
      */
     
     Members:
     
       CXCompletionChunk_Optional : /**
        * A code-completion string that describes "optional" text that
        * could be a part of the template (but is not required).
        *
        * The Optional chunk is the only kind of chunk that has a code-completion
        * string for its representation, which is accessible via
-       * \c clang_getCompletionChunkCompletionString(). The code-completion string
+       * \\c clang_getCompletionChunkCompletionString(). The code-completion string
        * describes an additional part of the template that is completely optional.
        * For example, optional chunks can be used to describe the placeholders for
        * arguments that match up with defaulted function parameters, e.g. given:
        *
-       * \code
+       * \\code
        * void f(int x, float y = 3.14, double z = 2.71828);
-       * \endcode
+       * \\endcode
        *
        * The code-completion string for this function would contain:
        *   - a TypedText chunk for "f".
        *   - a LeftParen chunk for "(".
        *   - a Placeholder chunk for "int x"
        *   - an Optional chunk containing the remaining defaulted arguments, e.g.,
        *       - a Comma chunk for ","
@@ -897,22 +1128,22 @@
        * Text that describes the current parameter when code-completion is
        * referring to function call, message send, or template specialization.
        *
        * A "current parameter" chunk occurs when code-completion is providing
        * information about a parameter corresponding to the argument at the
        * code-completion point. For example, given a function
        *
-       * \code
+       * \\code
        * int add(int x, int y);
-       * \endcode
+       * \\endcode
        *
-       * and the source code \c add(, where the code-completion point is after the
+       * and the source code \\c add(, where the code-completion point is after the
        * "(", the code-completion string will contain a "current parameter" chunk
        * for "int x", indicating that the current argument will initialize that
-       * parameter. After typing further, to \c add(17, (where the code-completion
+       * parameter. After typing further, to \\c add(17, (where the code-completion
        * point is after the ","), the code-completion string will contain a
        * "current parameter" chunk to "int y".
        */
     
       CXCompletionChunk_LeftParen : /**
        * A left parenthesis ('('), used to initiate a function call or
        * signal the beginning of a function parameter list.
@@ -972,15 +1203,15 @@
        */
     
       CXCompletionChunk_HorizontalSpace : /**
        * Horizontal space (' ').
        */
     
       CXCompletionChunk_VerticalSpace : /**
-       * Vertical space ('\\n'), after which it is generally a good idea to
+       * Vertical space ('\\\\n'), after which it is generally a good idea to
        * perform indentation.
        */
     """
     CXCompletionChunk_Colon: typing.ClassVar[CXCompletionChunkKind]  # value = <CXCompletionChunkKind.CXCompletionChunk_Colon: 16>
     CXCompletionChunk_Comma: typing.ClassVar[CXCompletionChunkKind]  # value = <CXCompletionChunkKind.CXCompletionChunk_Comma: 14>
     CXCompletionChunk_CurrentParameter: typing.ClassVar[CXCompletionChunkKind]  # value = <CXCompletionChunkKind.CXCompletionChunk_CurrentParameter: 5>
     CXCompletionChunk_Equal: typing.ClassVar[CXCompletionChunkKind]  # value = <CXCompletionChunkKind.CXCompletionChunk_Equal: 18>
@@ -1270,15 +1501,15 @@
         /**
            * The kind of entity that this completion refers to.
            *
            * The cursor kind will be a macro, keyword, or a declaration (one of the
            * *Decl cursor kinds), describing the entity that the completion is
            * referring to.
            *
-           * \todo In the future, we would like to provide a full cursor, to allow
+           * \\todo In the future, we would like to provide a full cursor, to allow
            * the client to extract additional information from declaration.
            */
         """
     @CursorKind.setter
     def CursorKind(self, arg0: CXCursorKind) -> None:
         ...
 class CXCursor:
@@ -1345,31 +1576,31 @@
     
       CXCursor_FunctionDecl : /** A function. */
     
       CXCursor_VarDecl : /** A variable. */
     
       CXCursor_ParmDecl : /** A function or method parameter. */
     
-      CXCursor_ObjCInterfaceDecl : /** An Objective-C \@interface. */
+      CXCursor_ObjCInterfaceDecl : /** An Objective-C \\@interface. */
     
-      CXCursor_ObjCCategoryDecl : /** An Objective-C \@interface for a category. */
+      CXCursor_ObjCCategoryDecl : /** An Objective-C \\@interface for a category. */
     
-      CXCursor_ObjCProtocolDecl : /** An Objective-C \@protocol declaration. */
+      CXCursor_ObjCProtocolDecl : /** An Objective-C \\@protocol declaration. */
     
-      CXCursor_ObjCPropertyDecl : /** An Objective-C \@property declaration. */
+      CXCursor_ObjCPropertyDecl : /** An Objective-C \\@property declaration. */
     
       CXCursor_ObjCIvarDecl : /** An Objective-C instance variable. */
     
       CXCursor_ObjCInstanceMethodDecl : /** An Objective-C instance method. */
     
       CXCursor_ObjCClassMethodDecl : /** An Objective-C class method. */
     
-      CXCursor_ObjCImplementationDecl : /** An Objective-C \@implementation. */
+      CXCursor_ObjCImplementationDecl : /** An Objective-C \\@implementation. */
     
-      CXCursor_ObjCCategoryImplDecl : /** An Objective-C \@implementation for a category. */
+      CXCursor_ObjCCategoryImplDecl : /** An Objective-C \\@implementation for a category. */
     
       CXCursor_TypedefDecl : /** A typedef. */
     
       CXCursor_CXXMethod : /** A C++ class method. */
     
       CXCursor_Namespace : /** A C++ namespace. */
     
@@ -1397,17 +1628,17 @@
     
       CXCursor_UsingDirective : /** A C++ using directive. */
     
       CXCursor_UsingDeclaration : /** A C++ using declaration. */
     
       CXCursor_TypeAliasDecl : /** A C++ alias declaration */
     
-      CXCursor_ObjCSynthesizeDecl : /** An Objective-C \@synthesize definition. */
+      CXCursor_ObjCSynthesizeDecl : /** An Objective-C \\@synthesize definition. */
     
-      CXCursor_ObjCDynamicDecl : /** An Objective-C \@dynamic definition. */
+      CXCursor_ObjCDynamicDecl : /** An Objective-C \\@dynamic definition. */
     
       CXCursor_CXXAccessSpecifier : /** An access specifier. */
     
       CXCursor_FirstDecl : /** An access specifier. */
     
       CXCursor_LastDecl : /** An access specifier. */
     
@@ -1421,34 +1652,34 @@
     
       CXCursor_TypeRef : /**
        * A reference to a type declaration.
        *
        * A type reference occurs anywhere where a type is named but not
        * declared. For example, given:
        *
-       * \code
+       * \\code
        * typedef unsigned size_type;
        * size_type size;
-       * \endcode
+       * \\endcode
        *
        * The typedef is a declaration of size_type (CXCursor_TypedefDecl),
        * while the type of the variable "size" is referenced. The cursor
        * referenced by the type of size is the typedef for size_type.
        */
     
       CXCursor_CXXBaseSpecifier : /**
        * A reference to a type declaration.
        *
        * A type reference occurs anywhere where a type is named but not
        * declared. For example, given:
        *
-       * \code
+       * \\code
        * typedef unsigned size_type;
        * size_type size;
-       * \endcode
+       * \\endcode
        *
        * The typedef is a declaration of size_type (CXCursor_TypedefDecl),
        * while the type of the variable "size" is referenced. The cursor
        * referenced by the type of size is the typedef for size_type.
        */
     
       CXCursor_TemplateRef : /**
@@ -1467,32 +1698,32 @@
     
       CXCursor_LabelRef : /**
        * A reference to a labeled statement.
        *
        * This cursor kind is used to describe the jump to "start_over" in the
        * goto statement in the following example:
        *
-       * \code
+       * \\code
        *   start_over:
        *     ++counter;
        *
        *     goto start_over;
-       * \endcode
+       * \\endcode
        *
        * A label reference cursor refers to a label statement.
        */
     
       CXCursor_OverloadedDeclRef : /**
        * A reference to a set of overloaded functions or function templates
        * that has not yet been resolved to a specific function or function template.
        *
        * An overloaded declaration reference cursor occurs in C++ templates where
        * a dependent name refers to a function. For example:
        *
-       * \code
+       * \\code
        * template<typename T> void swap(T&, T&);
        *
        * struct X { ... };
        * void swap(X&, X&);
        *
        * template<typename T>
        * void reverse(T* first, T* last) {
@@ -1500,25 +1731,25 @@
        *     swap(*first, *--last);
        *     ++first;
        *   }
        * }
        *
        * struct Y { };
        * void swap(Y&, Y&);
-       * \endcode
+       * \\endcode
        *
        * Here, the identifier "swap" is associated with an overloaded declaration
        * reference. In the template definition, "swap" refers to either of the two
        * "swap" functions declared above, so both results will be available. At
        * instantiation time, "swap" may also refer to other functions found via
        * argument-dependent lookup (e.g., the "swap" function at the end of the
        * example).
        *
-       * The functions \c clang_getNumOverloadedDecls() and
-       * \c clang_getOverloadedDecl() can be used to retrieve the definitions
+       * The functions \\c clang_getNumOverloadedDecls() and
+       * \\c clang_getOverloadedDecl() can be used to retrieve the definitions
        * referenced by this cursor.
        */
     
       CXCursor_VariableRef : /**
        * A reference to a variable that occurs in some non-expression
        * context, e.g., a C++ lambda capture list.
        */
@@ -1648,17 +1879,17 @@
       CXCursor_CXXConstCastExpr : /** C++'s const_cast<> expression.
        */
     
       CXCursor_CXXFunctionalCastExpr : /** Represents an explicit C++ type conversion that uses "functional"
        * notion (C++ [expr.type.conv]).
        *
        * Example:
-       * \code
+       * \\code
        *   x = int(0.5);
-       * \endcode
+       * \\endcode
        */
     
       CXCursor_CXXTypeidExpr : /** A C++ typeid expression (C++ [expr.typeid]).
        */
     
       CXCursor_CXXBoolLiteralExpr : /** [C++ 2.13.5] C++ Boolean Literal.
        */
@@ -1685,67 +1916,67 @@
     
       CXCursor_UnaryExpr : /** A unary expression. (noexcept, sizeof, or other traits)
        */
     
       CXCursor_ObjCStringLiteral : /** An Objective-C string literal i.e. @"foo".
        */
     
-      CXCursor_ObjCEncodeExpr : /** An Objective-C \@encode expression.
+      CXCursor_ObjCEncodeExpr : /** An Objective-C \\@encode expression.
        */
     
-      CXCursor_ObjCSelectorExpr : /** An Objective-C \@selector expression.
+      CXCursor_ObjCSelectorExpr : /** An Objective-C \\@selector expression.
        */
     
-      CXCursor_ObjCProtocolExpr : /** An Objective-C \@protocol expression.
+      CXCursor_ObjCProtocolExpr : /** An Objective-C \\@protocol expression.
        */
     
       CXCursor_ObjCBridgedCastExpr : /** An Objective-C "bridged" cast expression, which casts between
        * Objective-C pointers and C pointers, transferring ownership in the process.
        *
-       * \code
+       * \\code
        *   NSString *str = (__bridge_transfer NSString *)CFCreateString();
-       * \endcode
+       * \\endcode
        */
     
       CXCursor_PackExpansionExpr : /** Represents a C++0x pack expansion that produces a sequence of
        * expressions.
        *
        * A pack expansion expression contains a pattern (which itself is an
        * expression) followed by an ellipsis. For example:
        *
-       * \code
+       * \\code
        * template<typename F, typename ...Types>
        * void forward(F f, Types &&...args) {
        *  f(static_cast<Types&&>(args)...);
        * }
-       * \endcode
+       * \\endcode
        */
     
       CXCursor_SizeOfPackExpr : /** Represents an expression that computes the length of a parameter
        * pack.
        *
-       * \code
+       * \\code
        * template<typename ...Types>
        * struct count {
        *   static const unsigned value = sizeof...(Types);
        * };
-       * \endcode
+       * \\endcode
        */
     
       CXCursor_LambdaExpr : /* Represents a C++ lambda expression that produces a local function
        * object.
        *
-       * \code
+       * \\code
        * void abssort(float *x, unsigned N) {
        *   std::sort(x, x + N,
        *             [](float a, float b) {
        *               return std::abs(a) < std::abs(b);
        *             });
        * }
-       * \endcode
+       * \\endcode
        */
     
       CXCursor_ObjCBoolLiteralExpr : /** Objective-c Boolean Literal.
        */
     
       CXCursor_ObjCSelfExpr : /** Represents the "self" expression in an Objective-C method.
        */
@@ -1801,18 +2032,18 @@
        */
     
       CXCursor_LabelStmt : /** A labelled statement in a function.
        *
        * This cursor kind is used to describe the "start_over:" label statement in
        * the following example:
        *
-       * \code
+       * \\code
        *   start_over:
        *     ++counter;
-       * \endcode
+       * \\endcode
        *
        */
     
       CXCursor_CompoundStmt : /** A group of statements like { stmt stmt }.
        *
        * This cursor kind is used to describe compound statements, e.g. function
        * bodies.
@@ -1856,27 +2087,27 @@
     
       CXCursor_GCCAsmStmt : /** A GCC inline assembly statement extension.
        */
     
       CXCursor_AsmStmt : /** A GCC inline assembly statement extension.
        */
     
-      CXCursor_ObjCAtTryStmt : /** Objective-C's overall \@try-\@catch-\@finally statement.
+      CXCursor_ObjCAtTryStmt : /** Objective-C's overall \\@try-\\@catch-\\@finally statement.
        */
     
-      CXCursor_ObjCAtCatchStmt : /** Objective-C's \@catch statement.
+      CXCursor_ObjCAtCatchStmt : /** Objective-C's \\@catch statement.
        */
     
-      CXCursor_ObjCAtFinallyStmt : /** Objective-C's \@finally statement.
+      CXCursor_ObjCAtFinallyStmt : /** Objective-C's \\@finally statement.
        */
     
-      CXCursor_ObjCAtThrowStmt : /** Objective-C's \@throw statement.
+      CXCursor_ObjCAtThrowStmt : /** Objective-C's \\@throw statement.
        */
     
-      CXCursor_ObjCAtSynchronizedStmt : /** Objective-C's \@synchronized statement.
+      CXCursor_ObjCAtSynchronizedStmt : /** Objective-C's \\@synchronized statement.
        */
     
       CXCursor_ObjCAutoreleasePoolStmt : /** Objective-C's autorelease pool statement.
        */
     
       CXCursor_ObjCForCollectionStmt : /** Objective-C's collection statement.
        */
@@ -2129,15 +2360,18 @@
     
       CXCursor_OMPParallelMaskedTaskLoopSimdDirective : /** OpenMP parallel masked taskloop simd directive.
        */
     
       CXCursor_OMPErrorDirective : /** OpenMP error directive.
        */
     
-      CXCursor_LastStmt : /** OpenMP error directive.
+      CXCursor_OMPScopeDirective : /** OpenMP scope directive.
+       */
+    
+      CXCursor_LastStmt : /** OpenMP scope directive.
        */
     
       CXCursor_TranslationUnit : /**
        * Cursor that represents the translation unit itself.
        *
        * The translation unit cursor exists primarily to act as the root
        * cursor for traversing the contents of a translation unit.
@@ -2509,15 +2743,15 @@
     CXCursor_LastAttr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_AlignedAttr: 441>
     CXCursor_LastDecl: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_CXXAccessSpecifier: 39>
     CXCursor_LastExpr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_CXXParenListInitExpr: 155>
     CXCursor_LastExtraDecl: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_ConceptDecl: 604>
     CXCursor_LastInvalid: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_InvalidCode: 73>
     CXCursor_LastPreprocessing: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_InclusionDirective: 503>
     CXCursor_LastRef: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_VariableRef: 50>
-    CXCursor_LastStmt: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPErrorDirective: 305>
+    CXCursor_LastStmt: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPScopeDirective: 306>
     CXCursor_LinkageSpec: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_LinkageSpec: 23>
     CXCursor_MSAsmStmt: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MSAsmStmt: 229>
     CXCursor_MacroDefinition: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MacroDefinition: 501>
     CXCursor_MacroExpansion: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MacroExpansion: 502>
     CXCursor_MacroInstantiation: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MacroExpansion: 502>
     CXCursor_MemberRef: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MemberRef: 47>
     CXCursor_MemberRefExpr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_MemberRefExpr: 102>
@@ -2572,14 +2806,15 @@
     CXCursor_OMPParallelMaskedTaskLoopDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopDirective: 303>
     CXCursor_OMPParallelMaskedTaskLoopSimdDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopSimdDirective: 304>
     CXCursor_OMPParallelMasterDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelMasterDirective: 285>
     CXCursor_OMPParallelMasterTaskLoopDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopDirective: 282>
     CXCursor_OMPParallelMasterTaskLoopSimdDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopSimdDirective: 284>
     CXCursor_OMPParallelSectionsDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPParallelSectionsDirective: 239>
     CXCursor_OMPScanDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPScanDirective: 287>
+    CXCursor_OMPScopeDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPScopeDirective: 306>
     CXCursor_OMPSectionDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPSectionDirective: 236>
     CXCursor_OMPSectionsDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPSectionsDirective: 235>
     CXCursor_OMPSimdDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPSimdDirective: 233>
     CXCursor_OMPSingleDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPSingleDirective: 237>
     CXCursor_OMPTargetDataDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPTargetDataDirective: 257>
     CXCursor_OMPTargetDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPTargetDirective: 252>
     CXCursor_OMPTargetEnterDataDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_OMPTargetEnterDataDirective: 261>
@@ -2691,15 +2926,15 @@
     CXCursor_UsingDirective: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_UsingDirective: 34>
     CXCursor_VarDecl: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_VarDecl: 9>
     CXCursor_VariableRef: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_VariableRef: 50>
     CXCursor_VisibilityAttr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_VisibilityAttr: 417>
     CXCursor_WarnUnusedAttr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_WarnUnusedAttr: 439>
     CXCursor_WarnUnusedResultAttr: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_WarnUnusedResultAttr: 440>
     CXCursor_WhileStmt: typing.ClassVar[CXCursorKind]  # value = <CXCursorKind.CXCursor_WhileStmt: 207>
-    __members__: typing.ClassVar[dict[str, CXCursorKind]]  # value = {'CXCursor_UnexposedDecl': <CXCursorKind.CXCursor_UnexposedDecl: 1>, 'CXCursor_StructDecl': <CXCursorKind.CXCursor_StructDecl: 2>, 'CXCursor_UnionDecl': <CXCursorKind.CXCursor_UnionDecl: 3>, 'CXCursor_ClassDecl': <CXCursorKind.CXCursor_ClassDecl: 4>, 'CXCursor_EnumDecl': <CXCursorKind.CXCursor_EnumDecl: 5>, 'CXCursor_FieldDecl': <CXCursorKind.CXCursor_FieldDecl: 6>, 'CXCursor_EnumConstantDecl': <CXCursorKind.CXCursor_EnumConstantDecl: 7>, 'CXCursor_FunctionDecl': <CXCursorKind.CXCursor_FunctionDecl: 8>, 'CXCursor_VarDecl': <CXCursorKind.CXCursor_VarDecl: 9>, 'CXCursor_ParmDecl': <CXCursorKind.CXCursor_ParmDecl: 10>, 'CXCursor_ObjCInterfaceDecl': <CXCursorKind.CXCursor_ObjCInterfaceDecl: 11>, 'CXCursor_ObjCCategoryDecl': <CXCursorKind.CXCursor_ObjCCategoryDecl: 12>, 'CXCursor_ObjCProtocolDecl': <CXCursorKind.CXCursor_ObjCProtocolDecl: 13>, 'CXCursor_ObjCPropertyDecl': <CXCursorKind.CXCursor_ObjCPropertyDecl: 14>, 'CXCursor_ObjCIvarDecl': <CXCursorKind.CXCursor_ObjCIvarDecl: 15>, 'CXCursor_ObjCInstanceMethodDecl': <CXCursorKind.CXCursor_ObjCInstanceMethodDecl: 16>, 'CXCursor_ObjCClassMethodDecl': <CXCursorKind.CXCursor_ObjCClassMethodDecl: 17>, 'CXCursor_ObjCImplementationDecl': <CXCursorKind.CXCursor_ObjCImplementationDecl: 18>, 'CXCursor_ObjCCategoryImplDecl': <CXCursorKind.CXCursor_ObjCCategoryImplDecl: 19>, 'CXCursor_TypedefDecl': <CXCursorKind.CXCursor_TypedefDecl: 20>, 'CXCursor_CXXMethod': <CXCursorKind.CXCursor_CXXMethod: 21>, 'CXCursor_Namespace': <CXCursorKind.CXCursor_Namespace: 22>, 'CXCursor_LinkageSpec': <CXCursorKind.CXCursor_LinkageSpec: 23>, 'CXCursor_Constructor': <CXCursorKind.CXCursor_Constructor: 24>, 'CXCursor_Destructor': <CXCursorKind.CXCursor_Destructor: 25>, 'CXCursor_ConversionFunction': <CXCursorKind.CXCursor_ConversionFunction: 26>, 'CXCursor_TemplateTypeParameter': <CXCursorKind.CXCursor_TemplateTypeParameter: 27>, 'CXCursor_NonTypeTemplateParameter': <CXCursorKind.CXCursor_NonTypeTemplateParameter: 28>, 'CXCursor_TemplateTemplateParameter': <CXCursorKind.CXCursor_TemplateTemplateParameter: 29>, 'CXCursor_FunctionTemplate': <CXCursorKind.CXCursor_FunctionTemplate: 30>, 'CXCursor_ClassTemplate': <CXCursorKind.CXCursor_ClassTemplate: 31>, 'CXCursor_ClassTemplatePartialSpecialization': <CXCursorKind.CXCursor_ClassTemplatePartialSpecialization: 32>, 'CXCursor_NamespaceAlias': <CXCursorKind.CXCursor_NamespaceAlias: 33>, 'CXCursor_UsingDirective': <CXCursorKind.CXCursor_UsingDirective: 34>, 'CXCursor_UsingDeclaration': <CXCursorKind.CXCursor_UsingDeclaration: 35>, 'CXCursor_TypeAliasDecl': <CXCursorKind.CXCursor_TypeAliasDecl: 36>, 'CXCursor_ObjCSynthesizeDecl': <CXCursorKind.CXCursor_ObjCSynthesizeDecl: 37>, 'CXCursor_ObjCDynamicDecl': <CXCursorKind.CXCursor_ObjCDynamicDecl: 38>, 'CXCursor_CXXAccessSpecifier': <CXCursorKind.CXCursor_CXXAccessSpecifier: 39>, 'CXCursor_FirstDecl': <CXCursorKind.CXCursor_UnexposedDecl: 1>, 'CXCursor_LastDecl': <CXCursorKind.CXCursor_CXXAccessSpecifier: 39>, 'CXCursor_FirstRef': <CXCursorKind.CXCursor_FirstRef: 40>, 'CXCursor_ObjCSuperClassRef': <CXCursorKind.CXCursor_FirstRef: 40>, 'CXCursor_ObjCProtocolRef': <CXCursorKind.CXCursor_ObjCProtocolRef: 41>, 'CXCursor_ObjCClassRef': <CXCursorKind.CXCursor_ObjCClassRef: 42>, 'CXCursor_TypeRef': <CXCursorKind.CXCursor_TypeRef: 43>, 'CXCursor_CXXBaseSpecifier': <CXCursorKind.CXCursor_CXXBaseSpecifier: 44>, 'CXCursor_TemplateRef': <CXCursorKind.CXCursor_TemplateRef: 45>, 'CXCursor_NamespaceRef': <CXCursorKind.CXCursor_NamespaceRef: 46>, 'CXCursor_MemberRef': <CXCursorKind.CXCursor_MemberRef: 47>, 'CXCursor_LabelRef': <CXCursorKind.CXCursor_LabelRef: 48>, 'CXCursor_OverloadedDeclRef': <CXCursorKind.CXCursor_OverloadedDeclRef: 49>, 'CXCursor_VariableRef': <CXCursorKind.CXCursor_VariableRef: 50>, 'CXCursor_LastRef': <CXCursorKind.CXCursor_VariableRef: 50>, 'CXCursor_FirstInvalid': <CXCursorKind.CXCursor_FirstInvalid: 70>, 'CXCursor_InvalidFile': <CXCursorKind.CXCursor_FirstInvalid: 70>, 'CXCursor_NoDeclFound': <CXCursorKind.CXCursor_NoDeclFound: 71>, 'CXCursor_NotImplemented': <CXCursorKind.CXCursor_NotImplemented: 72>, 'CXCursor_InvalidCode': <CXCursorKind.CXCursor_InvalidCode: 73>, 'CXCursor_LastInvalid': <CXCursorKind.CXCursor_InvalidCode: 73>, 'CXCursor_FirstExpr': <CXCursorKind.CXCursor_FirstExpr: 100>, 'CXCursor_UnexposedExpr': <CXCursorKind.CXCursor_FirstExpr: 100>, 'CXCursor_DeclRefExpr': <CXCursorKind.CXCursor_DeclRefExpr: 101>, 'CXCursor_MemberRefExpr': <CXCursorKind.CXCursor_MemberRefExpr: 102>, 'CXCursor_CallExpr': <CXCursorKind.CXCursor_CallExpr: 103>, 'CXCursor_ObjCMessageExpr': <CXCursorKind.CXCursor_ObjCMessageExpr: 104>, 'CXCursor_BlockExpr': <CXCursorKind.CXCursor_BlockExpr: 105>, 'CXCursor_IntegerLiteral': <CXCursorKind.CXCursor_IntegerLiteral: 106>, 'CXCursor_FloatingLiteral': <CXCursorKind.CXCursor_FloatingLiteral: 107>, 'CXCursor_ImaginaryLiteral': <CXCursorKind.CXCursor_ImaginaryLiteral: 108>, 'CXCursor_StringLiteral': <CXCursorKind.CXCursor_StringLiteral: 109>, 'CXCursor_CharacterLiteral': <CXCursorKind.CXCursor_CharacterLiteral: 110>, 'CXCursor_ParenExpr': <CXCursorKind.CXCursor_ParenExpr: 111>, 'CXCursor_UnaryOperator': <CXCursorKind.CXCursor_UnaryOperator: 112>, 'CXCursor_ArraySubscriptExpr': <CXCursorKind.CXCursor_ArraySubscriptExpr: 113>, 'CXCursor_BinaryOperator': <CXCursorKind.CXCursor_BinaryOperator: 114>, 'CXCursor_CompoundAssignOperator': <CXCursorKind.CXCursor_CompoundAssignOperator: 115>, 'CXCursor_ConditionalOperator': <CXCursorKind.CXCursor_ConditionalOperator: 116>, 'CXCursor_CStyleCastExpr': <CXCursorKind.CXCursor_CStyleCastExpr: 117>, 'CXCursor_CompoundLiteralExpr': <CXCursorKind.CXCursor_CompoundLiteralExpr: 118>, 'CXCursor_InitListExpr': <CXCursorKind.CXCursor_InitListExpr: 119>, 'CXCursor_AddrLabelExpr': <CXCursorKind.CXCursor_AddrLabelExpr: 120>, 'CXCursor_StmtExpr': <CXCursorKind.CXCursor_StmtExpr: 121>, 'CXCursor_GenericSelectionExpr': <CXCursorKind.CXCursor_GenericSelectionExpr: 122>, 'CXCursor_GNUNullExpr': <CXCursorKind.CXCursor_GNUNullExpr: 123>, 'CXCursor_CXXStaticCastExpr': <CXCursorKind.CXCursor_CXXStaticCastExpr: 124>, 'CXCursor_CXXDynamicCastExpr': <CXCursorKind.CXCursor_CXXDynamicCastExpr: 125>, 'CXCursor_CXXReinterpretCastExpr': <CXCursorKind.CXCursor_CXXReinterpretCastExpr: 126>, 'CXCursor_CXXConstCastExpr': <CXCursorKind.CXCursor_CXXConstCastExpr: 127>, 'CXCursor_CXXFunctionalCastExpr': <CXCursorKind.CXCursor_CXXFunctionalCastExpr: 128>, 'CXCursor_CXXTypeidExpr': <CXCursorKind.CXCursor_CXXTypeidExpr: 129>, 'CXCursor_CXXBoolLiteralExpr': <CXCursorKind.CXCursor_CXXBoolLiteralExpr: 130>, 'CXCursor_CXXNullPtrLiteralExpr': <CXCursorKind.CXCursor_CXXNullPtrLiteralExpr: 131>, 'CXCursor_CXXThisExpr': <CXCursorKind.CXCursor_CXXThisExpr: 132>, 'CXCursor_CXXThrowExpr': <CXCursorKind.CXCursor_CXXThrowExpr: 133>, 'CXCursor_CXXNewExpr': <CXCursorKind.CXCursor_CXXNewExpr: 134>, 'CXCursor_CXXDeleteExpr': <CXCursorKind.CXCursor_CXXDeleteExpr: 135>, 'CXCursor_UnaryExpr': <CXCursorKind.CXCursor_UnaryExpr: 136>, 'CXCursor_ObjCStringLiteral': <CXCursorKind.CXCursor_ObjCStringLiteral: 137>, 'CXCursor_ObjCEncodeExpr': <CXCursorKind.CXCursor_ObjCEncodeExpr: 138>, 'CXCursor_ObjCSelectorExpr': <CXCursorKind.CXCursor_ObjCSelectorExpr: 139>, 'CXCursor_ObjCProtocolExpr': <CXCursorKind.CXCursor_ObjCProtocolExpr: 140>, 'CXCursor_ObjCBridgedCastExpr': <CXCursorKind.CXCursor_ObjCBridgedCastExpr: 141>, 'CXCursor_PackExpansionExpr': <CXCursorKind.CXCursor_PackExpansionExpr: 142>, 'CXCursor_SizeOfPackExpr': <CXCursorKind.CXCursor_SizeOfPackExpr: 143>, 'CXCursor_LambdaExpr': <CXCursorKind.CXCursor_LambdaExpr: 144>, 'CXCursor_ObjCBoolLiteralExpr': <CXCursorKind.CXCursor_ObjCBoolLiteralExpr: 145>, 'CXCursor_ObjCSelfExpr': <CXCursorKind.CXCursor_ObjCSelfExpr: 146>, 'CXCursor_OMPArraySectionExpr': <CXCursorKind.CXCursor_OMPArraySectionExpr: 147>, 'CXCursor_ObjCAvailabilityCheckExpr': <CXCursorKind.CXCursor_ObjCAvailabilityCheckExpr: 148>, 'CXCursor_FixedPointLiteral': <CXCursorKind.CXCursor_FixedPointLiteral: 149>, 'CXCursor_OMPArrayShapingExpr': <CXCursorKind.CXCursor_OMPArrayShapingExpr: 150>, 'CXCursor_OMPIteratorExpr': <CXCursorKind.CXCursor_OMPIteratorExpr: 151>, 'CXCursor_CXXAddrspaceCastExpr': <CXCursorKind.CXCursor_CXXAddrspaceCastExpr: 152>, 'CXCursor_ConceptSpecializationExpr': <CXCursorKind.CXCursor_ConceptSpecializationExpr: 153>, 'CXCursor_RequiresExpr': <CXCursorKind.CXCursor_RequiresExpr: 154>, 'CXCursor_CXXParenListInitExpr': <CXCursorKind.CXCursor_CXXParenListInitExpr: 155>, 'CXCursor_LastExpr': <CXCursorKind.CXCursor_CXXParenListInitExpr: 155>, 'CXCursor_FirstStmt': <CXCursorKind.CXCursor_FirstStmt: 200>, 'CXCursor_UnexposedStmt': <CXCursorKind.CXCursor_FirstStmt: 200>, 'CXCursor_LabelStmt': <CXCursorKind.CXCursor_LabelStmt: 201>, 'CXCursor_CompoundStmt': <CXCursorKind.CXCursor_CompoundStmt: 202>, 'CXCursor_CaseStmt': <CXCursorKind.CXCursor_CaseStmt: 203>, 'CXCursor_DefaultStmt': <CXCursorKind.CXCursor_DefaultStmt: 204>, 'CXCursor_IfStmt': <CXCursorKind.CXCursor_IfStmt: 205>, 'CXCursor_SwitchStmt': <CXCursorKind.CXCursor_SwitchStmt: 206>, 'CXCursor_WhileStmt': <CXCursorKind.CXCursor_WhileStmt: 207>, 'CXCursor_DoStmt': <CXCursorKind.CXCursor_DoStmt: 208>, 'CXCursor_ForStmt': <CXCursorKind.CXCursor_ForStmt: 209>, 'CXCursor_GotoStmt': <CXCursorKind.CXCursor_GotoStmt: 210>, 'CXCursor_IndirectGotoStmt': <CXCursorKind.CXCursor_IndirectGotoStmt: 211>, 'CXCursor_ContinueStmt': <CXCursorKind.CXCursor_ContinueStmt: 212>, 'CXCursor_BreakStmt': <CXCursorKind.CXCursor_BreakStmt: 213>, 'CXCursor_ReturnStmt': <CXCursorKind.CXCursor_ReturnStmt: 214>, 'CXCursor_GCCAsmStmt': <CXCursorKind.CXCursor_GCCAsmStmt: 215>, 'CXCursor_AsmStmt': <CXCursorKind.CXCursor_GCCAsmStmt: 215>, 'CXCursor_ObjCAtTryStmt': <CXCursorKind.CXCursor_ObjCAtTryStmt: 216>, 'CXCursor_ObjCAtCatchStmt': <CXCursorKind.CXCursor_ObjCAtCatchStmt: 217>, 'CXCursor_ObjCAtFinallyStmt': <CXCursorKind.CXCursor_ObjCAtFinallyStmt: 218>, 'CXCursor_ObjCAtThrowStmt': <CXCursorKind.CXCursor_ObjCAtThrowStmt: 219>, 'CXCursor_ObjCAtSynchronizedStmt': <CXCursorKind.CXCursor_ObjCAtSynchronizedStmt: 220>, 'CXCursor_ObjCAutoreleasePoolStmt': <CXCursorKind.CXCursor_ObjCAutoreleasePoolStmt: 221>, 'CXCursor_ObjCForCollectionStmt': <CXCursorKind.CXCursor_ObjCForCollectionStmt: 222>, 'CXCursor_CXXCatchStmt': <CXCursorKind.CXCursor_CXXCatchStmt: 223>, 'CXCursor_CXXTryStmt': <CXCursorKind.CXCursor_CXXTryStmt: 224>, 'CXCursor_CXXForRangeStmt': <CXCursorKind.CXCursor_CXXForRangeStmt: 225>, 'CXCursor_SEHTryStmt': <CXCursorKind.CXCursor_SEHTryStmt: 226>, 'CXCursor_SEHExceptStmt': <CXCursorKind.CXCursor_SEHExceptStmt: 227>, 'CXCursor_SEHFinallyStmt': <CXCursorKind.CXCursor_SEHFinallyStmt: 228>, 'CXCursor_MSAsmStmt': <CXCursorKind.CXCursor_MSAsmStmt: 229>, 'CXCursor_NullStmt': <CXCursorKind.CXCursor_NullStmt: 230>, 'CXCursor_DeclStmt': <CXCursorKind.CXCursor_DeclStmt: 231>, 'CXCursor_OMPParallelDirective': <CXCursorKind.CXCursor_OMPParallelDirective: 232>, 'CXCursor_OMPSimdDirective': <CXCursorKind.CXCursor_OMPSimdDirective: 233>, 'CXCursor_OMPForDirective': <CXCursorKind.CXCursor_OMPForDirective: 234>, 'CXCursor_OMPSectionsDirective': <CXCursorKind.CXCursor_OMPSectionsDirective: 235>, 'CXCursor_OMPSectionDirective': <CXCursorKind.CXCursor_OMPSectionDirective: 236>, 'CXCursor_OMPSingleDirective': <CXCursorKind.CXCursor_OMPSingleDirective: 237>, 'CXCursor_OMPParallelForDirective': <CXCursorKind.CXCursor_OMPParallelForDirective: 238>, 'CXCursor_OMPParallelSectionsDirective': <CXCursorKind.CXCursor_OMPParallelSectionsDirective: 239>, 'CXCursor_OMPTaskDirective': <CXCursorKind.CXCursor_OMPTaskDirective: 240>, 'CXCursor_OMPMasterDirective': <CXCursorKind.CXCursor_OMPMasterDirective: 241>, 'CXCursor_OMPCriticalDirective': <CXCursorKind.CXCursor_OMPCriticalDirective: 242>, 'CXCursor_OMPTaskyieldDirective': <CXCursorKind.CXCursor_OMPTaskyieldDirective: 243>, 'CXCursor_OMPBarrierDirective': <CXCursorKind.CXCursor_OMPBarrierDirective: 244>, 'CXCursor_OMPTaskwaitDirective': <CXCursorKind.CXCursor_OMPTaskwaitDirective: 245>, 'CXCursor_OMPFlushDirective': <CXCursorKind.CXCursor_OMPFlushDirective: 246>, 'CXCursor_SEHLeaveStmt': <CXCursorKind.CXCursor_SEHLeaveStmt: 247>, 'CXCursor_OMPOrderedDirective': <CXCursorKind.CXCursor_OMPOrderedDirective: 248>, 'CXCursor_OMPAtomicDirective': <CXCursorKind.CXCursor_OMPAtomicDirective: 249>, 'CXCursor_OMPForSimdDirective': <CXCursorKind.CXCursor_OMPForSimdDirective: 250>, 'CXCursor_OMPParallelForSimdDirective': <CXCursorKind.CXCursor_OMPParallelForSimdDirective: 251>, 'CXCursor_OMPTargetDirective': <CXCursorKind.CXCursor_OMPTargetDirective: 252>, 'CXCursor_OMPTeamsDirective': <CXCursorKind.CXCursor_OMPTeamsDirective: 253>, 'CXCursor_OMPTaskgroupDirective': <CXCursorKind.CXCursor_OMPTaskgroupDirective: 254>, 'CXCursor_OMPCancellationPointDirective': <CXCursorKind.CXCursor_OMPCancellationPointDirective: 255>, 'CXCursor_OMPCancelDirective': <CXCursorKind.CXCursor_OMPCancelDirective: 256>, 'CXCursor_OMPTargetDataDirective': <CXCursorKind.CXCursor_OMPTargetDataDirective: 257>, 'CXCursor_OMPTaskLoopDirective': <CXCursorKind.CXCursor_OMPTaskLoopDirective: 258>, 'CXCursor_OMPTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPTaskLoopSimdDirective: 259>, 'CXCursor_OMPDistributeDirective': <CXCursorKind.CXCursor_OMPDistributeDirective: 260>, 'CXCursor_OMPTargetEnterDataDirective': <CXCursorKind.CXCursor_OMPTargetEnterDataDirective: 261>, 'CXCursor_OMPTargetExitDataDirective': <CXCursorKind.CXCursor_OMPTargetExitDataDirective: 262>, 'CXCursor_OMPTargetParallelDirective': <CXCursorKind.CXCursor_OMPTargetParallelDirective: 263>, 'CXCursor_OMPTargetParallelForDirective': <CXCursorKind.CXCursor_OMPTargetParallelForDirective: 264>, 'CXCursor_OMPTargetUpdateDirective': <CXCursorKind.CXCursor_OMPTargetUpdateDirective: 265>, 'CXCursor_OMPDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPDistributeParallelForDirective: 266>, 'CXCursor_OMPDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPDistributeParallelForSimdDirective: 267>, 'CXCursor_OMPDistributeSimdDirective': <CXCursorKind.CXCursor_OMPDistributeSimdDirective: 268>, 'CXCursor_OMPTargetParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTargetParallelForSimdDirective: 269>, 'CXCursor_OMPTargetSimdDirective': <CXCursorKind.CXCursor_OMPTargetSimdDirective: 270>, 'CXCursor_OMPTeamsDistributeDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeDirective: 271>, 'CXCursor_OMPTeamsDistributeSimdDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeSimdDirective: 272>, 'CXCursor_OMPTeamsDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeParallelForSimdDirective: 273>, 'CXCursor_OMPTeamsDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeParallelForDirective: 274>, 'CXCursor_OMPTargetTeamsDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDirective: 275>, 'CXCursor_OMPTargetTeamsDistributeDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeDirective: 276>, 'CXCursor_OMPTargetTeamsDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeParallelForDirective: 277>, 'CXCursor_OMPTargetTeamsDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeParallelForSimdDirective: 278>, 'CXCursor_OMPTargetTeamsDistributeSimdDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeSimdDirective: 279>, 'CXCursor_BuiltinBitCastExpr': <CXCursorKind.CXCursor_BuiltinBitCastExpr: 280>, 'CXCursor_OMPMasterTaskLoopDirective': <CXCursorKind.CXCursor_OMPMasterTaskLoopDirective: 281>, 'CXCursor_OMPParallelMasterTaskLoopDirective': <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopDirective: 282>, 'CXCursor_OMPMasterTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPMasterTaskLoopSimdDirective: 283>, 'CXCursor_OMPParallelMasterTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopSimdDirective: 284>, 'CXCursor_OMPParallelMasterDirective': <CXCursorKind.CXCursor_OMPParallelMasterDirective: 285>, 'CXCursor_OMPDepobjDirective': <CXCursorKind.CXCursor_OMPDepobjDirective: 286>, 'CXCursor_OMPScanDirective': <CXCursorKind.CXCursor_OMPScanDirective: 287>, 'CXCursor_OMPTileDirective': <CXCursorKind.CXCursor_OMPTileDirective: 288>, 'CXCursor_OMPCanonicalLoop': <CXCursorKind.CXCursor_OMPCanonicalLoop: 289>, 'CXCursor_OMPInteropDirective': <CXCursorKind.CXCursor_OMPInteropDirective: 290>, 'CXCursor_OMPDispatchDirective': <CXCursorKind.CXCursor_OMPDispatchDirective: 291>, 'CXCursor_OMPMaskedDirective': <CXCursorKind.CXCursor_OMPMaskedDirective: 292>, 'CXCursor_OMPUnrollDirective': <CXCursorKind.CXCursor_OMPUnrollDirective: 293>, 'CXCursor_OMPMetaDirective': <CXCursorKind.CXCursor_OMPMetaDirective: 294>, 'CXCursor_OMPGenericLoopDirective': <CXCursorKind.CXCursor_OMPGenericLoopDirective: 295>, 'CXCursor_OMPTeamsGenericLoopDirective': <CXCursorKind.CXCursor_OMPTeamsGenericLoopDirective: 296>, 'CXCursor_OMPTargetTeamsGenericLoopDirective': <CXCursorKind.CXCursor_OMPTargetTeamsGenericLoopDirective: 297>, 'CXCursor_OMPParallelGenericLoopDirective': <CXCursorKind.CXCursor_OMPParallelGenericLoopDirective: 298>, 'CXCursor_OMPTargetParallelGenericLoopDirective': <CXCursorKind.CXCursor_OMPTargetParallelGenericLoopDirective: 299>, 'CXCursor_OMPParallelMaskedDirective': <CXCursorKind.CXCursor_OMPParallelMaskedDirective: 300>, 'CXCursor_OMPMaskedTaskLoopDirective': <CXCursorKind.CXCursor_OMPMaskedTaskLoopDirective: 301>, 'CXCursor_OMPMaskedTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPMaskedTaskLoopSimdDirective: 302>, 'CXCursor_OMPParallelMaskedTaskLoopDirective': <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopDirective: 303>, 'CXCursor_OMPParallelMaskedTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopSimdDirective: 304>, 'CXCursor_OMPErrorDirective': <CXCursorKind.CXCursor_OMPErrorDirective: 305>, 'CXCursor_LastStmt': <CXCursorKind.CXCursor_OMPErrorDirective: 305>, 'CXCursor_TranslationUnit': <CXCursorKind.CXCursor_TranslationUnit: 350>, 'CXCursor_FirstAttr': <CXCursorKind.CXCursor_FirstAttr: 400>, 'CXCursor_UnexposedAttr': <CXCursorKind.CXCursor_FirstAttr: 400>, 'CXCursor_IBActionAttr': <CXCursorKind.CXCursor_IBActionAttr: 401>, 'CXCursor_IBOutletAttr': <CXCursorKind.CXCursor_IBOutletAttr: 402>, 'CXCursor_IBOutletCollectionAttr': <CXCursorKind.CXCursor_IBOutletCollectionAttr: 403>, 'CXCursor_CXXFinalAttr': <CXCursorKind.CXCursor_CXXFinalAttr: 404>, 'CXCursor_CXXOverrideAttr': <CXCursorKind.CXCursor_CXXOverrideAttr: 405>, 'CXCursor_AnnotateAttr': <CXCursorKind.CXCursor_AnnotateAttr: 406>, 'CXCursor_AsmLabelAttr': <CXCursorKind.CXCursor_AsmLabelAttr: 407>, 'CXCursor_PackedAttr': <CXCursorKind.CXCursor_PackedAttr: 408>, 'CXCursor_PureAttr': <CXCursorKind.CXCursor_PureAttr: 409>, 'CXCursor_ConstAttr': <CXCursorKind.CXCursor_ConstAttr: 410>, 'CXCursor_NoDuplicateAttr': <CXCursorKind.CXCursor_NoDuplicateAttr: 411>, 'CXCursor_CUDAConstantAttr': <CXCursorKind.CXCursor_CUDAConstantAttr: 412>, 'CXCursor_CUDADeviceAttr': <CXCursorKind.CXCursor_CUDADeviceAttr: 413>, 'CXCursor_CUDAGlobalAttr': <CXCursorKind.CXCursor_CUDAGlobalAttr: 414>, 'CXCursor_CUDAHostAttr': <CXCursorKind.CXCursor_CUDAHostAttr: 415>, 'CXCursor_CUDASharedAttr': <CXCursorKind.CXCursor_CUDASharedAttr: 416>, 'CXCursor_VisibilityAttr': <CXCursorKind.CXCursor_VisibilityAttr: 417>, 'CXCursor_DLLExport': <CXCursorKind.CXCursor_DLLExport: 418>, 'CXCursor_DLLImport': <CXCursorKind.CXCursor_DLLImport: 419>, 'CXCursor_NSReturnsRetained': <CXCursorKind.CXCursor_NSReturnsRetained: 420>, 'CXCursor_NSReturnsNotRetained': <CXCursorKind.CXCursor_NSReturnsNotRetained: 421>, 'CXCursor_NSReturnsAutoreleased': <CXCursorKind.CXCursor_NSReturnsAutoreleased: 422>, 'CXCursor_NSConsumesSelf': <CXCursorKind.CXCursor_NSConsumesSelf: 423>, 'CXCursor_NSConsumed': <CXCursorKind.CXCursor_NSConsumed: 424>, 'CXCursor_ObjCException': <CXCursorKind.CXCursor_ObjCException: 425>, 'CXCursor_ObjCNSObject': <CXCursorKind.CXCursor_ObjCNSObject: 426>, 'CXCursor_ObjCIndependentClass': <CXCursorKind.CXCursor_ObjCIndependentClass: 427>, 'CXCursor_ObjCPreciseLifetime': <CXCursorKind.CXCursor_ObjCPreciseLifetime: 428>, 'CXCursor_ObjCReturnsInnerPointer': <CXCursorKind.CXCursor_ObjCReturnsInnerPointer: 429>, 'CXCursor_ObjCRequiresSuper': <CXCursorKind.CXCursor_ObjCRequiresSuper: 430>, 'CXCursor_ObjCRootClass': <CXCursorKind.CXCursor_ObjCRootClass: 431>, 'CXCursor_ObjCSubclassingRestricted': <CXCursorKind.CXCursor_ObjCSubclassingRestricted: 432>, 'CXCursor_ObjCExplicitProtocolImpl': <CXCursorKind.CXCursor_ObjCExplicitProtocolImpl: 433>, 'CXCursor_ObjCDesignatedInitializer': <CXCursorKind.CXCursor_ObjCDesignatedInitializer: 434>, 'CXCursor_ObjCRuntimeVisible': <CXCursorKind.CXCursor_ObjCRuntimeVisible: 435>, 'CXCursor_ObjCBoxable': <CXCursorKind.CXCursor_ObjCBoxable: 436>, 'CXCursor_FlagEnum': <CXCursorKind.CXCursor_FlagEnum: 437>, 'CXCursor_ConvergentAttr': <CXCursorKind.CXCursor_ConvergentAttr: 438>, 'CXCursor_WarnUnusedAttr': <CXCursorKind.CXCursor_WarnUnusedAttr: 439>, 'CXCursor_WarnUnusedResultAttr': <CXCursorKind.CXCursor_WarnUnusedResultAttr: 440>, 'CXCursor_AlignedAttr': <CXCursorKind.CXCursor_AlignedAttr: 441>, 'CXCursor_LastAttr': <CXCursorKind.CXCursor_AlignedAttr: 441>, 'CXCursor_PreprocessingDirective': <CXCursorKind.CXCursor_PreprocessingDirective: 500>, 'CXCursor_MacroDefinition': <CXCursorKind.CXCursor_MacroDefinition: 501>, 'CXCursor_MacroExpansion': <CXCursorKind.CXCursor_MacroExpansion: 502>, 'CXCursor_MacroInstantiation': <CXCursorKind.CXCursor_MacroExpansion: 502>, 'CXCursor_InclusionDirective': <CXCursorKind.CXCursor_InclusionDirective: 503>, 'CXCursor_FirstPreprocessing': <CXCursorKind.CXCursor_PreprocessingDirective: 500>, 'CXCursor_LastPreprocessing': <CXCursorKind.CXCursor_InclusionDirective: 503>, 'CXCursor_ModuleImportDecl': <CXCursorKind.CXCursor_ModuleImportDecl: 600>, 'CXCursor_TypeAliasTemplateDecl': <CXCursorKind.CXCursor_TypeAliasTemplateDecl: 601>, 'CXCursor_StaticAssert': <CXCursorKind.CXCursor_StaticAssert: 602>, 'CXCursor_FriendDecl': <CXCursorKind.CXCursor_FriendDecl: 603>, 'CXCursor_ConceptDecl': <CXCursorKind.CXCursor_ConceptDecl: 604>, 'CXCursor_FirstExtraDecl': <CXCursorKind.CXCursor_ModuleImportDecl: 600>, 'CXCursor_LastExtraDecl': <CXCursorKind.CXCursor_ConceptDecl: 604>, 'CXCursor_OverloadCandidate': <CXCursorKind.CXCursor_OverloadCandidate: 700>}
+    __members__: typing.ClassVar[dict[str, CXCursorKind]]  # value = {'CXCursor_UnexposedDecl': <CXCursorKind.CXCursor_UnexposedDecl: 1>, 'CXCursor_StructDecl': <CXCursorKind.CXCursor_StructDecl: 2>, 'CXCursor_UnionDecl': <CXCursorKind.CXCursor_UnionDecl: 3>, 'CXCursor_ClassDecl': <CXCursorKind.CXCursor_ClassDecl: 4>, 'CXCursor_EnumDecl': <CXCursorKind.CXCursor_EnumDecl: 5>, 'CXCursor_FieldDecl': <CXCursorKind.CXCursor_FieldDecl: 6>, 'CXCursor_EnumConstantDecl': <CXCursorKind.CXCursor_EnumConstantDecl: 7>, 'CXCursor_FunctionDecl': <CXCursorKind.CXCursor_FunctionDecl: 8>, 'CXCursor_VarDecl': <CXCursorKind.CXCursor_VarDecl: 9>, 'CXCursor_ParmDecl': <CXCursorKind.CXCursor_ParmDecl: 10>, 'CXCursor_ObjCInterfaceDecl': <CXCursorKind.CXCursor_ObjCInterfaceDecl: 11>, 'CXCursor_ObjCCategoryDecl': <CXCursorKind.CXCursor_ObjCCategoryDecl: 12>, 'CXCursor_ObjCProtocolDecl': <CXCursorKind.CXCursor_ObjCProtocolDecl: 13>, 'CXCursor_ObjCPropertyDecl': <CXCursorKind.CXCursor_ObjCPropertyDecl: 14>, 'CXCursor_ObjCIvarDecl': <CXCursorKind.CXCursor_ObjCIvarDecl: 15>, 'CXCursor_ObjCInstanceMethodDecl': <CXCursorKind.CXCursor_ObjCInstanceMethodDecl: 16>, 'CXCursor_ObjCClassMethodDecl': <CXCursorKind.CXCursor_ObjCClassMethodDecl: 17>, 'CXCursor_ObjCImplementationDecl': <CXCursorKind.CXCursor_ObjCImplementationDecl: 18>, 'CXCursor_ObjCCategoryImplDecl': <CXCursorKind.CXCursor_ObjCCategoryImplDecl: 19>, 'CXCursor_TypedefDecl': <CXCursorKind.CXCursor_TypedefDecl: 20>, 'CXCursor_CXXMethod': <CXCursorKind.CXCursor_CXXMethod: 21>, 'CXCursor_Namespace': <CXCursorKind.CXCursor_Namespace: 22>, 'CXCursor_LinkageSpec': <CXCursorKind.CXCursor_LinkageSpec: 23>, 'CXCursor_Constructor': <CXCursorKind.CXCursor_Constructor: 24>, 'CXCursor_Destructor': <CXCursorKind.CXCursor_Destructor: 25>, 'CXCursor_ConversionFunction': <CXCursorKind.CXCursor_ConversionFunction: 26>, 'CXCursor_TemplateTypeParameter': <CXCursorKind.CXCursor_TemplateTypeParameter: 27>, 'CXCursor_NonTypeTemplateParameter': <CXCursorKind.CXCursor_NonTypeTemplateParameter: 28>, 'CXCursor_TemplateTemplateParameter': <CXCursorKind.CXCursor_TemplateTemplateParameter: 29>, 'CXCursor_FunctionTemplate': <CXCursorKind.CXCursor_FunctionTemplate: 30>, 'CXCursor_ClassTemplate': <CXCursorKind.CXCursor_ClassTemplate: 31>, 'CXCursor_ClassTemplatePartialSpecialization': <CXCursorKind.CXCursor_ClassTemplatePartialSpecialization: 32>, 'CXCursor_NamespaceAlias': <CXCursorKind.CXCursor_NamespaceAlias: 33>, 'CXCursor_UsingDirective': <CXCursorKind.CXCursor_UsingDirective: 34>, 'CXCursor_UsingDeclaration': <CXCursorKind.CXCursor_UsingDeclaration: 35>, 'CXCursor_TypeAliasDecl': <CXCursorKind.CXCursor_TypeAliasDecl: 36>, 'CXCursor_ObjCSynthesizeDecl': <CXCursorKind.CXCursor_ObjCSynthesizeDecl: 37>, 'CXCursor_ObjCDynamicDecl': <CXCursorKind.CXCursor_ObjCDynamicDecl: 38>, 'CXCursor_CXXAccessSpecifier': <CXCursorKind.CXCursor_CXXAccessSpecifier: 39>, 'CXCursor_FirstDecl': <CXCursorKind.CXCursor_UnexposedDecl: 1>, 'CXCursor_LastDecl': <CXCursorKind.CXCursor_CXXAccessSpecifier: 39>, 'CXCursor_FirstRef': <CXCursorKind.CXCursor_FirstRef: 40>, 'CXCursor_ObjCSuperClassRef': <CXCursorKind.CXCursor_FirstRef: 40>, 'CXCursor_ObjCProtocolRef': <CXCursorKind.CXCursor_ObjCProtocolRef: 41>, 'CXCursor_ObjCClassRef': <CXCursorKind.CXCursor_ObjCClassRef: 42>, 'CXCursor_TypeRef': <CXCursorKind.CXCursor_TypeRef: 43>, 'CXCursor_CXXBaseSpecifier': <CXCursorKind.CXCursor_CXXBaseSpecifier: 44>, 'CXCursor_TemplateRef': <CXCursorKind.CXCursor_TemplateRef: 45>, 'CXCursor_NamespaceRef': <CXCursorKind.CXCursor_NamespaceRef: 46>, 'CXCursor_MemberRef': <CXCursorKind.CXCursor_MemberRef: 47>, 'CXCursor_LabelRef': <CXCursorKind.CXCursor_LabelRef: 48>, 'CXCursor_OverloadedDeclRef': <CXCursorKind.CXCursor_OverloadedDeclRef: 49>, 'CXCursor_VariableRef': <CXCursorKind.CXCursor_VariableRef: 50>, 'CXCursor_LastRef': <CXCursorKind.CXCursor_VariableRef: 50>, 'CXCursor_FirstInvalid': <CXCursorKind.CXCursor_FirstInvalid: 70>, 'CXCursor_InvalidFile': <CXCursorKind.CXCursor_FirstInvalid: 70>, 'CXCursor_NoDeclFound': <CXCursorKind.CXCursor_NoDeclFound: 71>, 'CXCursor_NotImplemented': <CXCursorKind.CXCursor_NotImplemented: 72>, 'CXCursor_InvalidCode': <CXCursorKind.CXCursor_InvalidCode: 73>, 'CXCursor_LastInvalid': <CXCursorKind.CXCursor_InvalidCode: 73>, 'CXCursor_FirstExpr': <CXCursorKind.CXCursor_FirstExpr: 100>, 'CXCursor_UnexposedExpr': <CXCursorKind.CXCursor_FirstExpr: 100>, 'CXCursor_DeclRefExpr': <CXCursorKind.CXCursor_DeclRefExpr: 101>, 'CXCursor_MemberRefExpr': <CXCursorKind.CXCursor_MemberRefExpr: 102>, 'CXCursor_CallExpr': <CXCursorKind.CXCursor_CallExpr: 103>, 'CXCursor_ObjCMessageExpr': <CXCursorKind.CXCursor_ObjCMessageExpr: 104>, 'CXCursor_BlockExpr': <CXCursorKind.CXCursor_BlockExpr: 105>, 'CXCursor_IntegerLiteral': <CXCursorKind.CXCursor_IntegerLiteral: 106>, 'CXCursor_FloatingLiteral': <CXCursorKind.CXCursor_FloatingLiteral: 107>, 'CXCursor_ImaginaryLiteral': <CXCursorKind.CXCursor_ImaginaryLiteral: 108>, 'CXCursor_StringLiteral': <CXCursorKind.CXCursor_StringLiteral: 109>, 'CXCursor_CharacterLiteral': <CXCursorKind.CXCursor_CharacterLiteral: 110>, 'CXCursor_ParenExpr': <CXCursorKind.CXCursor_ParenExpr: 111>, 'CXCursor_UnaryOperator': <CXCursorKind.CXCursor_UnaryOperator: 112>, 'CXCursor_ArraySubscriptExpr': <CXCursorKind.CXCursor_ArraySubscriptExpr: 113>, 'CXCursor_BinaryOperator': <CXCursorKind.CXCursor_BinaryOperator: 114>, 'CXCursor_CompoundAssignOperator': <CXCursorKind.CXCursor_CompoundAssignOperator: 115>, 'CXCursor_ConditionalOperator': <CXCursorKind.CXCursor_ConditionalOperator: 116>, 'CXCursor_CStyleCastExpr': <CXCursorKind.CXCursor_CStyleCastExpr: 117>, 'CXCursor_CompoundLiteralExpr': <CXCursorKind.CXCursor_CompoundLiteralExpr: 118>, 'CXCursor_InitListExpr': <CXCursorKind.CXCursor_InitListExpr: 119>, 'CXCursor_AddrLabelExpr': <CXCursorKind.CXCursor_AddrLabelExpr: 120>, 'CXCursor_StmtExpr': <CXCursorKind.CXCursor_StmtExpr: 121>, 'CXCursor_GenericSelectionExpr': <CXCursorKind.CXCursor_GenericSelectionExpr: 122>, 'CXCursor_GNUNullExpr': <CXCursorKind.CXCursor_GNUNullExpr: 123>, 'CXCursor_CXXStaticCastExpr': <CXCursorKind.CXCursor_CXXStaticCastExpr: 124>, 'CXCursor_CXXDynamicCastExpr': <CXCursorKind.CXCursor_CXXDynamicCastExpr: 125>, 'CXCursor_CXXReinterpretCastExpr': <CXCursorKind.CXCursor_CXXReinterpretCastExpr: 126>, 'CXCursor_CXXConstCastExpr': <CXCursorKind.CXCursor_CXXConstCastExpr: 127>, 'CXCursor_CXXFunctionalCastExpr': <CXCursorKind.CXCursor_CXXFunctionalCastExpr: 128>, 'CXCursor_CXXTypeidExpr': <CXCursorKind.CXCursor_CXXTypeidExpr: 129>, 'CXCursor_CXXBoolLiteralExpr': <CXCursorKind.CXCursor_CXXBoolLiteralExpr: 130>, 'CXCursor_CXXNullPtrLiteralExpr': <CXCursorKind.CXCursor_CXXNullPtrLiteralExpr: 131>, 'CXCursor_CXXThisExpr': <CXCursorKind.CXCursor_CXXThisExpr: 132>, 'CXCursor_CXXThrowExpr': <CXCursorKind.CXCursor_CXXThrowExpr: 133>, 'CXCursor_CXXNewExpr': <CXCursorKind.CXCursor_CXXNewExpr: 134>, 'CXCursor_CXXDeleteExpr': <CXCursorKind.CXCursor_CXXDeleteExpr: 135>, 'CXCursor_UnaryExpr': <CXCursorKind.CXCursor_UnaryExpr: 136>, 'CXCursor_ObjCStringLiteral': <CXCursorKind.CXCursor_ObjCStringLiteral: 137>, 'CXCursor_ObjCEncodeExpr': <CXCursorKind.CXCursor_ObjCEncodeExpr: 138>, 'CXCursor_ObjCSelectorExpr': <CXCursorKind.CXCursor_ObjCSelectorExpr: 139>, 'CXCursor_ObjCProtocolExpr': <CXCursorKind.CXCursor_ObjCProtocolExpr: 140>, 'CXCursor_ObjCBridgedCastExpr': <CXCursorKind.CXCursor_ObjCBridgedCastExpr: 141>, 'CXCursor_PackExpansionExpr': <CXCursorKind.CXCursor_PackExpansionExpr: 142>, 'CXCursor_SizeOfPackExpr': <CXCursorKind.CXCursor_SizeOfPackExpr: 143>, 'CXCursor_LambdaExpr': <CXCursorKind.CXCursor_LambdaExpr: 144>, 'CXCursor_ObjCBoolLiteralExpr': <CXCursorKind.CXCursor_ObjCBoolLiteralExpr: 145>, 'CXCursor_ObjCSelfExpr': <CXCursorKind.CXCursor_ObjCSelfExpr: 146>, 'CXCursor_OMPArraySectionExpr': <CXCursorKind.CXCursor_OMPArraySectionExpr: 147>, 'CXCursor_ObjCAvailabilityCheckExpr': <CXCursorKind.CXCursor_ObjCAvailabilityCheckExpr: 148>, 'CXCursor_FixedPointLiteral': <CXCursorKind.CXCursor_FixedPointLiteral: 149>, 'CXCursor_OMPArrayShapingExpr': <CXCursorKind.CXCursor_OMPArrayShapingExpr: 150>, 'CXCursor_OMPIteratorExpr': <CXCursorKind.CXCursor_OMPIteratorExpr: 151>, 'CXCursor_CXXAddrspaceCastExpr': <CXCursorKind.CXCursor_CXXAddrspaceCastExpr: 152>, 'CXCursor_ConceptSpecializationExpr': <CXCursorKind.CXCursor_ConceptSpecializationExpr: 153>, 'CXCursor_RequiresExpr': <CXCursorKind.CXCursor_RequiresExpr: 154>, 'CXCursor_CXXParenListInitExpr': <CXCursorKind.CXCursor_CXXParenListInitExpr: 155>, 'CXCursor_LastExpr': <CXCursorKind.CXCursor_CXXParenListInitExpr: 155>, 'CXCursor_FirstStmt': <CXCursorKind.CXCursor_FirstStmt: 200>, 'CXCursor_UnexposedStmt': <CXCursorKind.CXCursor_FirstStmt: 200>, 'CXCursor_LabelStmt': <CXCursorKind.CXCursor_LabelStmt: 201>, 'CXCursor_CompoundStmt': <CXCursorKind.CXCursor_CompoundStmt: 202>, 'CXCursor_CaseStmt': <CXCursorKind.CXCursor_CaseStmt: 203>, 'CXCursor_DefaultStmt': <CXCursorKind.CXCursor_DefaultStmt: 204>, 'CXCursor_IfStmt': <CXCursorKind.CXCursor_IfStmt: 205>, 'CXCursor_SwitchStmt': <CXCursorKind.CXCursor_SwitchStmt: 206>, 'CXCursor_WhileStmt': <CXCursorKind.CXCursor_WhileStmt: 207>, 'CXCursor_DoStmt': <CXCursorKind.CXCursor_DoStmt: 208>, 'CXCursor_ForStmt': <CXCursorKind.CXCursor_ForStmt: 209>, 'CXCursor_GotoStmt': <CXCursorKind.CXCursor_GotoStmt: 210>, 'CXCursor_IndirectGotoStmt': <CXCursorKind.CXCursor_IndirectGotoStmt: 211>, 'CXCursor_ContinueStmt': <CXCursorKind.CXCursor_ContinueStmt: 212>, 'CXCursor_BreakStmt': <CXCursorKind.CXCursor_BreakStmt: 213>, 'CXCursor_ReturnStmt': <CXCursorKind.CXCursor_ReturnStmt: 214>, 'CXCursor_GCCAsmStmt': <CXCursorKind.CXCursor_GCCAsmStmt: 215>, 'CXCursor_AsmStmt': <CXCursorKind.CXCursor_GCCAsmStmt: 215>, 'CXCursor_ObjCAtTryStmt': <CXCursorKind.CXCursor_ObjCAtTryStmt: 216>, 'CXCursor_ObjCAtCatchStmt': <CXCursorKind.CXCursor_ObjCAtCatchStmt: 217>, 'CXCursor_ObjCAtFinallyStmt': <CXCursorKind.CXCursor_ObjCAtFinallyStmt: 218>, 'CXCursor_ObjCAtThrowStmt': <CXCursorKind.CXCursor_ObjCAtThrowStmt: 219>, 'CXCursor_ObjCAtSynchronizedStmt': <CXCursorKind.CXCursor_ObjCAtSynchronizedStmt: 220>, 'CXCursor_ObjCAutoreleasePoolStmt': <CXCursorKind.CXCursor_ObjCAutoreleasePoolStmt: 221>, 'CXCursor_ObjCForCollectionStmt': <CXCursorKind.CXCursor_ObjCForCollectionStmt: 222>, 'CXCursor_CXXCatchStmt': <CXCursorKind.CXCursor_CXXCatchStmt: 223>, 'CXCursor_CXXTryStmt': <CXCursorKind.CXCursor_CXXTryStmt: 224>, 'CXCursor_CXXForRangeStmt': <CXCursorKind.CXCursor_CXXForRangeStmt: 225>, 'CXCursor_SEHTryStmt': <CXCursorKind.CXCursor_SEHTryStmt: 226>, 'CXCursor_SEHExceptStmt': <CXCursorKind.CXCursor_SEHExceptStmt: 227>, 'CXCursor_SEHFinallyStmt': <CXCursorKind.CXCursor_SEHFinallyStmt: 228>, 'CXCursor_MSAsmStmt': <CXCursorKind.CXCursor_MSAsmStmt: 229>, 'CXCursor_NullStmt': <CXCursorKind.CXCursor_NullStmt: 230>, 'CXCursor_DeclStmt': <CXCursorKind.CXCursor_DeclStmt: 231>, 'CXCursor_OMPParallelDirective': <CXCursorKind.CXCursor_OMPParallelDirective: 232>, 'CXCursor_OMPSimdDirective': <CXCursorKind.CXCursor_OMPSimdDirective: 233>, 'CXCursor_OMPForDirective': <CXCursorKind.CXCursor_OMPForDirective: 234>, 'CXCursor_OMPSectionsDirective': <CXCursorKind.CXCursor_OMPSectionsDirective: 235>, 'CXCursor_OMPSectionDirective': <CXCursorKind.CXCursor_OMPSectionDirective: 236>, 'CXCursor_OMPSingleDirective': <CXCursorKind.CXCursor_OMPSingleDirective: 237>, 'CXCursor_OMPParallelForDirective': <CXCursorKind.CXCursor_OMPParallelForDirective: 238>, 'CXCursor_OMPParallelSectionsDirective': <CXCursorKind.CXCursor_OMPParallelSectionsDirective: 239>, 'CXCursor_OMPTaskDirective': <CXCursorKind.CXCursor_OMPTaskDirective: 240>, 'CXCursor_OMPMasterDirective': <CXCursorKind.CXCursor_OMPMasterDirective: 241>, 'CXCursor_OMPCriticalDirective': <CXCursorKind.CXCursor_OMPCriticalDirective: 242>, 'CXCursor_OMPTaskyieldDirective': <CXCursorKind.CXCursor_OMPTaskyieldDirective: 243>, 'CXCursor_OMPBarrierDirective': <CXCursorKind.CXCursor_OMPBarrierDirective: 244>, 'CXCursor_OMPTaskwaitDirective': <CXCursorKind.CXCursor_OMPTaskwaitDirective: 245>, 'CXCursor_OMPFlushDirective': <CXCursorKind.CXCursor_OMPFlushDirective: 246>, 'CXCursor_SEHLeaveStmt': <CXCursorKind.CXCursor_SEHLeaveStmt: 247>, 'CXCursor_OMPOrderedDirective': <CXCursorKind.CXCursor_OMPOrderedDirective: 248>, 'CXCursor_OMPAtomicDirective': <CXCursorKind.CXCursor_OMPAtomicDirective: 249>, 'CXCursor_OMPForSimdDirective': <CXCursorKind.CXCursor_OMPForSimdDirective: 250>, 'CXCursor_OMPParallelForSimdDirective': <CXCursorKind.CXCursor_OMPParallelForSimdDirective: 251>, 'CXCursor_OMPTargetDirective': <CXCursorKind.CXCursor_OMPTargetDirective: 252>, 'CXCursor_OMPTeamsDirective': <CXCursorKind.CXCursor_OMPTeamsDirective: 253>, 'CXCursor_OMPTaskgroupDirective': <CXCursorKind.CXCursor_OMPTaskgroupDirective: 254>, 'CXCursor_OMPCancellationPointDirective': <CXCursorKind.CXCursor_OMPCancellationPointDirective: 255>, 'CXCursor_OMPCancelDirective': <CXCursorKind.CXCursor_OMPCancelDirective: 256>, 'CXCursor_OMPTargetDataDirective': <CXCursorKind.CXCursor_OMPTargetDataDirective: 257>, 'CXCursor_OMPTaskLoopDirective': <CXCursorKind.CXCursor_OMPTaskLoopDirective: 258>, 'CXCursor_OMPTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPTaskLoopSimdDirective: 259>, 'CXCursor_OMPDistributeDirective': <CXCursorKind.CXCursor_OMPDistributeDirective: 260>, 'CXCursor_OMPTargetEnterDataDirective': <CXCursorKind.CXCursor_OMPTargetEnterDataDirective: 261>, 'CXCursor_OMPTargetExitDataDirective': <CXCursorKind.CXCursor_OMPTargetExitDataDirective: 262>, 'CXCursor_OMPTargetParallelDirective': <CXCursorKind.CXCursor_OMPTargetParallelDirective: 263>, 'CXCursor_OMPTargetParallelForDirective': <CXCursorKind.CXCursor_OMPTargetParallelForDirective: 264>, 'CXCursor_OMPTargetUpdateDirective': <CXCursorKind.CXCursor_OMPTargetUpdateDirective: 265>, 'CXCursor_OMPDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPDistributeParallelForDirective: 266>, 'CXCursor_OMPDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPDistributeParallelForSimdDirective: 267>, 'CXCursor_OMPDistributeSimdDirective': <CXCursorKind.CXCursor_OMPDistributeSimdDirective: 268>, 'CXCursor_OMPTargetParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTargetParallelForSimdDirective: 269>, 'CXCursor_OMPTargetSimdDirective': <CXCursorKind.CXCursor_OMPTargetSimdDirective: 270>, 'CXCursor_OMPTeamsDistributeDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeDirective: 271>, 'CXCursor_OMPTeamsDistributeSimdDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeSimdDirective: 272>, 'CXCursor_OMPTeamsDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeParallelForSimdDirective: 273>, 'CXCursor_OMPTeamsDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPTeamsDistributeParallelForDirective: 274>, 'CXCursor_OMPTargetTeamsDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDirective: 275>, 'CXCursor_OMPTargetTeamsDistributeDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeDirective: 276>, 'CXCursor_OMPTargetTeamsDistributeParallelForDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeParallelForDirective: 277>, 'CXCursor_OMPTargetTeamsDistributeParallelForSimdDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeParallelForSimdDirective: 278>, 'CXCursor_OMPTargetTeamsDistributeSimdDirective': <CXCursorKind.CXCursor_OMPTargetTeamsDistributeSimdDirective: 279>, 'CXCursor_BuiltinBitCastExpr': <CXCursorKind.CXCursor_BuiltinBitCastExpr: 280>, 'CXCursor_OMPMasterTaskLoopDirective': <CXCursorKind.CXCursor_OMPMasterTaskLoopDirective: 281>, 'CXCursor_OMPParallelMasterTaskLoopDirective': <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopDirective: 282>, 'CXCursor_OMPMasterTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPMasterTaskLoopSimdDirective: 283>, 'CXCursor_OMPParallelMasterTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPParallelMasterTaskLoopSimdDirective: 284>, 'CXCursor_OMPParallelMasterDirective': <CXCursorKind.CXCursor_OMPParallelMasterDirective: 285>, 'CXCursor_OMPDepobjDirective': <CXCursorKind.CXCursor_OMPDepobjDirective: 286>, 'CXCursor_OMPScanDirective': <CXCursorKind.CXCursor_OMPScanDirective: 287>, 'CXCursor_OMPTileDirective': <CXCursorKind.CXCursor_OMPTileDirective: 288>, 'CXCursor_OMPCanonicalLoop': <CXCursorKind.CXCursor_OMPCanonicalLoop: 289>, 'CXCursor_OMPInteropDirective': <CXCursorKind.CXCursor_OMPInteropDirective: 290>, 'CXCursor_OMPDispatchDirective': <CXCursorKind.CXCursor_OMPDispatchDirective: 291>, 'CXCursor_OMPMaskedDirective': <CXCursorKind.CXCursor_OMPMaskedDirective: 292>, 'CXCursor_OMPUnrollDirective': <CXCursorKind.CXCursor_OMPUnrollDirective: 293>, 'CXCursor_OMPMetaDirective': <CXCursorKind.CXCursor_OMPMetaDirective: 294>, 'CXCursor_OMPGenericLoopDirective': <CXCursorKind.CXCursor_OMPGenericLoopDirective: 295>, 'CXCursor_OMPTeamsGenericLoopDirective': <CXCursorKind.CXCursor_OMPTeamsGenericLoopDirective: 296>, 'CXCursor_OMPTargetTeamsGenericLoopDirective': <CXCursorKind.CXCursor_OMPTargetTeamsGenericLoopDirective: 297>, 'CXCursor_OMPParallelGenericLoopDirective': <CXCursorKind.CXCursor_OMPParallelGenericLoopDirective: 298>, 'CXCursor_OMPTargetParallelGenericLoopDirective': <CXCursorKind.CXCursor_OMPTargetParallelGenericLoopDirective: 299>, 'CXCursor_OMPParallelMaskedDirective': <CXCursorKind.CXCursor_OMPParallelMaskedDirective: 300>, 'CXCursor_OMPMaskedTaskLoopDirective': <CXCursorKind.CXCursor_OMPMaskedTaskLoopDirective: 301>, 'CXCursor_OMPMaskedTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPMaskedTaskLoopSimdDirective: 302>, 'CXCursor_OMPParallelMaskedTaskLoopDirective': <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopDirective: 303>, 'CXCursor_OMPParallelMaskedTaskLoopSimdDirective': <CXCursorKind.CXCursor_OMPParallelMaskedTaskLoopSimdDirective: 304>, 'CXCursor_OMPErrorDirective': <CXCursorKind.CXCursor_OMPErrorDirective: 305>, 'CXCursor_OMPScopeDirective': <CXCursorKind.CXCursor_OMPScopeDirective: 306>, 'CXCursor_LastStmt': <CXCursorKind.CXCursor_OMPScopeDirective: 306>, 'CXCursor_TranslationUnit': <CXCursorKind.CXCursor_TranslationUnit: 350>, 'CXCursor_FirstAttr': <CXCursorKind.CXCursor_FirstAttr: 400>, 'CXCursor_UnexposedAttr': <CXCursorKind.CXCursor_FirstAttr: 400>, 'CXCursor_IBActionAttr': <CXCursorKind.CXCursor_IBActionAttr: 401>, 'CXCursor_IBOutletAttr': <CXCursorKind.CXCursor_IBOutletAttr: 402>, 'CXCursor_IBOutletCollectionAttr': <CXCursorKind.CXCursor_IBOutletCollectionAttr: 403>, 'CXCursor_CXXFinalAttr': <CXCursorKind.CXCursor_CXXFinalAttr: 404>, 'CXCursor_CXXOverrideAttr': <CXCursorKind.CXCursor_CXXOverrideAttr: 405>, 'CXCursor_AnnotateAttr': <CXCursorKind.CXCursor_AnnotateAttr: 406>, 'CXCursor_AsmLabelAttr': <CXCursorKind.CXCursor_AsmLabelAttr: 407>, 'CXCursor_PackedAttr': <CXCursorKind.CXCursor_PackedAttr: 408>, 'CXCursor_PureAttr': <CXCursorKind.CXCursor_PureAttr: 409>, 'CXCursor_ConstAttr': <CXCursorKind.CXCursor_ConstAttr: 410>, 'CXCursor_NoDuplicateAttr': <CXCursorKind.CXCursor_NoDuplicateAttr: 411>, 'CXCursor_CUDAConstantAttr': <CXCursorKind.CXCursor_CUDAConstantAttr: 412>, 'CXCursor_CUDADeviceAttr': <CXCursorKind.CXCursor_CUDADeviceAttr: 413>, 'CXCursor_CUDAGlobalAttr': <CXCursorKind.CXCursor_CUDAGlobalAttr: 414>, 'CXCursor_CUDAHostAttr': <CXCursorKind.CXCursor_CUDAHostAttr: 415>, 'CXCursor_CUDASharedAttr': <CXCursorKind.CXCursor_CUDASharedAttr: 416>, 'CXCursor_VisibilityAttr': <CXCursorKind.CXCursor_VisibilityAttr: 417>, 'CXCursor_DLLExport': <CXCursorKind.CXCursor_DLLExport: 418>, 'CXCursor_DLLImport': <CXCursorKind.CXCursor_DLLImport: 419>, 'CXCursor_NSReturnsRetained': <CXCursorKind.CXCursor_NSReturnsRetained: 420>, 'CXCursor_NSReturnsNotRetained': <CXCursorKind.CXCursor_NSReturnsNotRetained: 421>, 'CXCursor_NSReturnsAutoreleased': <CXCursorKind.CXCursor_NSReturnsAutoreleased: 422>, 'CXCursor_NSConsumesSelf': <CXCursorKind.CXCursor_NSConsumesSelf: 423>, 'CXCursor_NSConsumed': <CXCursorKind.CXCursor_NSConsumed: 424>, 'CXCursor_ObjCException': <CXCursorKind.CXCursor_ObjCException: 425>, 'CXCursor_ObjCNSObject': <CXCursorKind.CXCursor_ObjCNSObject: 426>, 'CXCursor_ObjCIndependentClass': <CXCursorKind.CXCursor_ObjCIndependentClass: 427>, 'CXCursor_ObjCPreciseLifetime': <CXCursorKind.CXCursor_ObjCPreciseLifetime: 428>, 'CXCursor_ObjCReturnsInnerPointer': <CXCursorKind.CXCursor_ObjCReturnsInnerPointer: 429>, 'CXCursor_ObjCRequiresSuper': <CXCursorKind.CXCursor_ObjCRequiresSuper: 430>, 'CXCursor_ObjCRootClass': <CXCursorKind.CXCursor_ObjCRootClass: 431>, 'CXCursor_ObjCSubclassingRestricted': <CXCursorKind.CXCursor_ObjCSubclassingRestricted: 432>, 'CXCursor_ObjCExplicitProtocolImpl': <CXCursorKind.CXCursor_ObjCExplicitProtocolImpl: 433>, 'CXCursor_ObjCDesignatedInitializer': <CXCursorKind.CXCursor_ObjCDesignatedInitializer: 434>, 'CXCursor_ObjCRuntimeVisible': <CXCursorKind.CXCursor_ObjCRuntimeVisible: 435>, 'CXCursor_ObjCBoxable': <CXCursorKind.CXCursor_ObjCBoxable: 436>, 'CXCursor_FlagEnum': <CXCursorKind.CXCursor_FlagEnum: 437>, 'CXCursor_ConvergentAttr': <CXCursorKind.CXCursor_ConvergentAttr: 438>, 'CXCursor_WarnUnusedAttr': <CXCursorKind.CXCursor_WarnUnusedAttr: 439>, 'CXCursor_WarnUnusedResultAttr': <CXCursorKind.CXCursor_WarnUnusedResultAttr: 440>, 'CXCursor_AlignedAttr': <CXCursorKind.CXCursor_AlignedAttr: 441>, 'CXCursor_LastAttr': <CXCursorKind.CXCursor_AlignedAttr: 441>, 'CXCursor_PreprocessingDirective': <CXCursorKind.CXCursor_PreprocessingDirective: 500>, 'CXCursor_MacroDefinition': <CXCursorKind.CXCursor_MacroDefinition: 501>, 'CXCursor_MacroExpansion': <CXCursorKind.CXCursor_MacroExpansion: 502>, 'CXCursor_MacroInstantiation': <CXCursorKind.CXCursor_MacroExpansion: 502>, 'CXCursor_InclusionDirective': <CXCursorKind.CXCursor_InclusionDirective: 503>, 'CXCursor_FirstPreprocessing': <CXCursorKind.CXCursor_PreprocessingDirective: 500>, 'CXCursor_LastPreprocessing': <CXCursorKind.CXCursor_InclusionDirective: 503>, 'CXCursor_ModuleImportDecl': <CXCursorKind.CXCursor_ModuleImportDecl: 600>, 'CXCursor_TypeAliasTemplateDecl': <CXCursorKind.CXCursor_TypeAliasTemplateDecl: 601>, 'CXCursor_StaticAssert': <CXCursorKind.CXCursor_StaticAssert: 602>, 'CXCursor_FriendDecl': <CXCursorKind.CXCursor_FriendDecl: 603>, 'CXCursor_ConceptDecl': <CXCursorKind.CXCursor_ConceptDecl: 604>, 'CXCursor_FirstExtraDecl': <CXCursorKind.CXCursor_ModuleImportDecl: 600>, 'CXCursor_LastExtraDecl': <CXCursorKind.CXCursor_ConceptDecl: 604>, 'CXCursor_OverloadCandidate': <CXCursorKind.CXCursor_OverloadCandidate: 700>}
     def __and__(self, other: typing.Any) -> typing.Any:
         ...
     def __eq__(self, other: typing.Any) -> bool:
         ...
     def __ge__(self, other: typing.Any) -> bool:
         ...
     def __getstate__(self) -> int:
@@ -2867,71 +3102,71 @@
         ...
 class CXDiagnosticDisplayOptions:
     """
     /**
      * Options to control the display of diagnostics.
      *
      * The values in this enum are meant to be combined to customize the
-     * behavior of \c clang_formatDiagnostic().
+     * behavior of \\c clang_formatDiagnostic().
      */
     
     Members:
     
       CXDiagnostic_DisplaySourceLocation : /**
        * Display the source-location information where the
        * diagnostic was located.
        *
        * When set, diagnostics will be prefixed by the file, line, and
        * (optionally) column to which the diagnostic refers. For example,
        *
-       * \code
+       * \\code
        * test.c:28: warning: extra tokens at end of #endif directive
-       * \endcode
+       * \\endcode
        *
-       * This option corresponds to the clang flag \c -fshow-source-location.
+       * This option corresponds to the clang flag \\c -fshow-source-location.
        */
     
       CXDiagnostic_DisplayColumn : /**
        * If displaying the source-location information of the
        * diagnostic, also include the column number.
        *
-       * This option corresponds to the clang flag \c -fshow-column.
+       * This option corresponds to the clang flag \\c -fshow-column.
        */
     
       CXDiagnostic_DisplaySourceRanges : /**
        * If displaying the source-location information of the
        * diagnostic, also include information about source ranges in a
        * machine-parsable format.
        *
        * This option corresponds to the clang flag
-       * \c -fdiagnostics-print-source-range-info.
+       * \\c -fdiagnostics-print-source-range-info.
        */
     
       CXDiagnostic_DisplayOption : /**
        * Display the option name associated with this diagnostic, if any.
        *
        * The option name displayed (e.g., -Wconversion) will be placed in brackets
        * after the diagnostic text. This option corresponds to the clang flag
-       * \c -fdiagnostics-show-option.
+       * \\c -fdiagnostics-show-option.
        */
     
       CXDiagnostic_DisplayCategoryId : /**
        * Display the category number associated with this diagnostic, if any.
        *
        * The category number is displayed within brackets after the diagnostic text.
        * This option corresponds to the clang flag
-       * \c -fdiagnostics-show-category=id.
+       * \\c -fdiagnostics-show-category=id.
        */
     
       CXDiagnostic_DisplayCategoryName : /**
        * Display the category name associated with this diagnostic, if any.
        *
        * The category name is displayed within brackets after the diagnostic text.
        * This option corresponds to the clang flag
-       * \c -fdiagnostics-show-category=name.
+       * \\c -fdiagnostics-show-category=name.
        */
     """
     CXDiagnostic_DisplayCategoryId: typing.ClassVar[CXDiagnosticDisplayOptions]  # value = <CXDiagnosticDisplayOptions.CXDiagnostic_DisplayCategoryId: 16>
     CXDiagnostic_DisplayCategoryName: typing.ClassVar[CXDiagnosticDisplayOptions]  # value = <CXDiagnosticDisplayOptions.CXDiagnostic_DisplayCategoryName: 32>
     CXDiagnostic_DisplayColumn: typing.ClassVar[CXDiagnosticDisplayOptions]  # value = <CXDiagnosticDisplayOptions.CXDiagnostic_DisplayColumn: 2>
     CXDiagnostic_DisplayOption: typing.ClassVar[CXDiagnosticDisplayOptions]  # value = <CXDiagnosticDisplayOptions.CXDiagnostic_DisplayOption: 8>
     CXDiagnostic_DisplaySourceLocation: typing.ClassVar[CXDiagnosticDisplayOptions]  # value = <CXDiagnosticDisplayOptions.CXDiagnostic_DisplaySourceLocation: 1>
@@ -3073,15 +3308,15 @@
     def value(self) -> int:
         ...
 class CXErrorCode:
     """
     /**
      * Error codes returned by libclang routines.
      *
-     * Zero (\c CXError_Success) is the only error code indicating success.  Other
+     * Zero (\\c CXError_Success) is the only error code indicating success.  Other
      * error codes, including not yet assigned non-zero values, indicate errors.
      */
     
     Members:
     
       CXError_Success : /**
        * No error.
@@ -3791,15 +4026,15 @@
         ...
 class CXIdxEntityRefKind:
     """
     /**
      * Data for IndexerCallbacks#indexEntityReference.
      *
      * This may be deprecated in a future version as this duplicates
-     * the \c CXSymbolRole_Implicit bit in \c CXSymbolRole.
+     * the \\c CXSymbolRole_Implicit bit in \\c CXSymbolRole.
      */
     
     Members:
     
       CXIdxEntityRef_Direct : /**
        * The entity is referenced directly in user's code.
        */
@@ -3892,15 +4127,15 @@
     isImport: int
     def __init__(self) -> None:
         ...
     @property
     def filename(self) -> str:
         """
         /**
-           * Filename as written in the \#include/\#import directive.
+           * Filename as written in the \\#include/\\#import directive.
            */
         """
     @filename.setter
     def filename(self, arg0: str) -> None:
         ...
     @property
     def isModuleImport(self) -> int:
@@ -4030,15 +4265,15 @@
     
       CXIndexOpt_SuppressWarnings : /**
        * Suppress all compiler warnings when parsing for indexing.
        */
     
       CXIndexOpt_SkipParsedBodiesInSession : /**
        * Skip a function/method body that was already parsed during an
-       * indexing session associated with a \c CXIndexAction object.
+       * indexing session associated with a \\c CXIndexAction object.
        * Bodies in system headers are always skipped.
        */
     """
     CXIndexOpt_IndexFunctionLocalSymbols: typing.ClassVar[CXIndexOptFlags]  # value = <CXIndexOptFlags.CXIndexOpt_IndexFunctionLocalSymbols: 2>
     CXIndexOpt_IndexImplicitTemplateInstantiations: typing.ClassVar[CXIndexOptFlags]  # value = <CXIndexOptFlags.CXIndexOpt_IndexImplicitTemplateInstantiations: 4>
     CXIndexOpt_None: typing.ClassVar[CXIndexOptFlags]  # value = <CXIndexOptFlags.CXIndexOpt_None: 0>
     CXIndexOpt_SkipParsedBodiesInSession: typing.ClassVar[CXIndexOptFlags]  # value = <CXIndexOptFlags.CXIndexOpt_SkipParsedBodiesInSession: 16>
@@ -4089,14 +4324,103 @@
         ...
     @property
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
+class CXIndexOptions:
+    """
+    /**
+     * Index initialization options.
+     *
+     * 0 is the default value of each member of this struct except for Size.
+     * Initialize the struct in one of the following three ways to avoid adapting
+     * code each time a new member is added to it:
+     * \\code
+     * CXIndexOptions Opts;
+     * memset(&Opts, 0, sizeof(Opts));
+     * Opts.Size = sizeof(CXIndexOptions);
+     * \\endcode
+     * or explicitly initialize the first data member and zero-initialize the rest:
+     * \\code
+     * CXIndexOptions Opts = { sizeof(CXIndexOptions) };
+     * \\endcode
+     * or to prevent the -Wmissing-field-initializers warning for the above version:
+     * \\code
+     * CXIndexOptions Opts{};
+     * Opts.Size = sizeof(CXIndexOptions);
+     * \\endcode
+     */
+    """
+    def __init__(self) -> None:
+        ...
+    @property
+    def InvocationEmissionPath(self) -> str:
+        """
+        /**
+           * Specifies a path which will contain log files for certain libclang
+           * invocations. A null value implies that libclang invocations are not logged.
+           */
+        """
+    @InvocationEmissionPath.setter
+    def InvocationEmissionPath(self, arg0: str) -> None:
+        ...
+    @property
+    def PreambleStoragePath(self) -> str:
+        """
+        /**
+           * The path to a directory, in which to store temporary PCH files. If null or
+           * empty, the default system temporary directory is used. These PCH files are
+           * deleted on clean exit but stay on disk if the program crashes or is killed.
+           *
+           * This option is ignored if \\a StorePreamblesInMemory is non-zero.
+           *
+           * Libclang does not create the directory at the specified path in the file
+           * system. Therefore it must exist, or storing PCH files will fail.
+           */
+        """
+    @PreambleStoragePath.setter
+    def PreambleStoragePath(self, arg0: str) -> None:
+        ...
+    @property
+    def Size(self) -> int:
+        """
+        /**
+           * The size of struct CXIndexOptions used for option versioning.
+           *
+           * Always initialize this member to sizeof(CXIndexOptions), or assign
+           * sizeof(CXIndexOptions) to it right after creating a CXIndexOptions object.
+           */
+        """
+    @Size.setter
+    def Size(self, arg0: int) -> None:
+        ...
+    @property
+    def ThreadBackgroundPriorityForEditing(self) -> int:
+        """
+        /**
+           * A CXChoice enumerator that specifies the editing priority policy.
+           * \\sa CXGlobalOpt_ThreadBackgroundPriorityForEditing
+           */
+        """
+    @ThreadBackgroundPriorityForEditing.setter
+    def ThreadBackgroundPriorityForEditing(self, arg0: int) -> None:
+        ...
+    @property
+    def ThreadBackgroundPriorityForIndexing(self) -> int:
+        """
+        /**
+           * A CXChoice enumerator that specifies the indexing priority policy.
+           * \\sa CXGlobalOpt_ThreadBackgroundPriorityForIndexing
+           */
+        """
+    @ThreadBackgroundPriorityForIndexing.setter
+    def ThreadBackgroundPriorityForIndexing(self, arg0: int) -> None:
+        ...
 class CXLanguageKind:
     """
     /**
      * Describe the "language" of the entity referred to by a cursor.
      */
     
     Members:
@@ -4239,15 +4563,15 @@
     @property
     def value(self) -> int:
         ...
 class CXLoadDiag_Error:
     """
     /**
      * Describes the kind of error that occurred (if any) in a call to
-     * \c clang_loadDiagnostics.
+     * \\c clang_loadDiagnostics.
      */
     
     Members:
     
       CXLoadDiag_None : /**
        * Indicates that no error occurred.
        */
@@ -4332,27 +4656,27 @@
     
       CXNameRange_WantQualifier : /**
        * Include the nested-name-specifier, e.g. Foo:: in x.Foo::y, in the
        * range.
        */
     
       CXNameRange_WantTemplateArgs : /**
-       * Include the explicit template arguments, e.g. \<int> in x.f<int>,
+       * Include the explicit template arguments, e.g. \\<int> in x.f<int>,
        * in the range.
        */
     
       CXNameRange_WantSinglePiece : /**
        * If the name is non-contiguous, return the full spanning range.
        *
        * Non-contiguous names occur in Objective-C when a selector with two or more
        * parameters is used, or in C++ when using an operator:
-       * \code
+       * \\code
        * [object doSomething:here withValue:there]; // Objective-C
        * return some_vector[1]; // C++
-       * \endcode
+       * \\endcode
        */
     """
     CXNameRange_WantQualifier: typing.ClassVar[CXNameRefFlags]  # value = <CXNameRefFlags.CXNameRange_WantQualifier: 1>
     CXNameRange_WantSinglePiece: typing.ClassVar[CXNameRefFlags]  # value = <CXNameRefFlags.CXNameRange_WantSinglePiece: 4>
     CXNameRange_WantTemplateArgs: typing.ClassVar[CXNameRefFlags]  # value = <CXNameRefFlags.CXNameRange_WantTemplateArgs: 2>
     __members__: typing.ClassVar[dict[str, CXNameRefFlags]]  # value = {'CXNameRange_WantQualifier': <CXNameRefFlags.CXNameRange_WantQualifier: 1>, 'CXNameRange_WantTemplateArgs': <CXNameRefFlags.CXNameRange_WantTemplateArgs: 2>, 'CXNameRange_WantSinglePiece': <CXNameRefFlags.CXNameRange_WantSinglePiece: 4>}
     def __and__(self, other: typing.Any) -> typing.Any:
@@ -4481,15 +4805,15 @@
         ...
     @property
     def value(self) -> int:
         ...
 class CXObjCPropertyAttrKind:
     """
     /**
-     * Property attributes for a \c CXCursor_ObjCPropertyDecl.
+     * Property attributes for a \\c CXCursor_ObjCPropertyDecl.
      */
     
     Members:
     
       CXObjCPropertyAttr_noattr
     
       CXObjCPropertyAttr_readonly
@@ -4601,15 +4925,15 @@
     def Unavailable(self, arg0: int) -> None:
         ...
 class CXPrintingPolicyProperty:
     """
     /**
      * Properties for the printing policy.
      *
-     * See \c clang::PrintingPolicy for more information.
+     * See \\c clang::PrintingPolicy for more information.
      */
     
     Members:
     
       CXPrintingPolicy_Indentation
     
       CXPrintingPolicy_SuppressSpecifiers
@@ -4742,17 +5066,17 @@
         ...
 class CXRefQualifierKind:
     """
     Members:
     
       CXRefQualifier_None : /** No ref-qualifier was provided. */
     
-      CXRefQualifier_LValue : /** An lvalue ref-qualifier was provided (\c &). */
+      CXRefQualifier_LValue : /** An lvalue ref-qualifier was provided (\\c &). */
     
-      CXRefQualifier_RValue : /** An rvalue ref-qualifier was provided (\c &&). */
+      CXRefQualifier_RValue : /** An rvalue ref-qualifier was provided (\\c &&). */
     """
     CXRefQualifier_LValue: typing.ClassVar[CXRefQualifierKind]  # value = <CXRefQualifierKind.CXRefQualifier_LValue: 1>
     CXRefQualifier_None: typing.ClassVar[CXRefQualifierKind]  # value = <CXRefQualifierKind.CXRefQualifier_None: 0>
     CXRefQualifier_RValue: typing.ClassVar[CXRefQualifierKind]  # value = <CXRefQualifierKind.CXRefQualifier_RValue: 2>
     __members__: typing.ClassVar[dict[str, CXRefQualifierKind]]  # value = {'CXRefQualifier_None': <CXRefQualifierKind.CXRefQualifier_None: 0>, 'CXRefQualifier_LValue': <CXRefQualifierKind.CXRefQualifier_LValue: 1>, 'CXRefQualifier_RValue': <CXRefQualifierKind.CXRefQualifier_RValue: 2>}
     def __and__(self, other: typing.Any) -> typing.Any:
         ...
@@ -4937,15 +5261,15 @@
     @property
     def value(self) -> int:
         ...
 class CXSaveError:
     """
     /**
      * Describes the kind of error that occurred (if any) in a call to
-     * \c clang_saveTranslationUnit().
+     * \\c clang_saveTranslationUnit().
      */
     
     Members:
     
       CXSaveError_None : /**
        * Indicates that no error occurred while saving a translation unit.
        */
@@ -4959,15 +5283,15 @@
        */
     
       CXSaveError_TranslationErrors : /**
        * Indicates that errors during translation prevented this attempt
        * to save the translation unit.
        *
        * Errors that prevent the translation unit from being saved can be
-       * extracted using \c clang_getNumDiagnostics() and \c clang_getDiagnostic().
+       * extracted using \\c clang_getNumDiagnostics() and \\c clang_getDiagnostic().
        */
     
       CXSaveError_InvalidTU : /**
        * Indicates that the translation unit to be saved was somehow
        * invalid (e.g., NULL).
        */
     """
@@ -5123,28 +5447,28 @@
      */
     """
     def __init__(self) -> None:
         ...
     @property
     def count(self) -> int:
         """
-        /** The number of ranges in the \c ranges array. */
+        /** The number of ranges in the \\c ranges array. */
         """
     @count.setter
     def count(self, arg0: int) -> None:
         ...
 class CXString:
     """
     /**
      * A character string.
      *
-     * The \c CXString type is used to return strings from the interface when
+     * The \\c CXString type is used to return strings from the interface when
      * the ownership of that string might differ from one call to the next.
-     * Use \c clang_getCString() to retrieve the string data and, once finished
-     * with the string data, call \c clang_disposeString() to free the string.
+     * Use \\c clang_getCString() to retrieve the string data and, once finished
+     * with the string data, call \\c clang_disposeString() to free the string.
      */
     """
     private_flags: int
     def __init__(self) -> None:
         ...
 class CXStringSet:
     Count: int
@@ -5704,15 +6028,15 @@
        *
        * An implicit precompiled header is used as an optimization when a
        * particular translation unit is likely to be reparsed many times
        * when the sources aren't changing that often. In this case, an
        * implicit precompiled header will be built containing all of the
        * initial includes at the top of the main file (what we refer to as
        * the "preamble" of the file). In subsequent parses, if the
-       * preamble or the files in it have not changed, \c
+       * preamble or the files in it have not changed, \\c
        * clang_reparseTranslationUnit() will re-use the implicit
        * precompiled header to improve parsing performance.
        */
     
       CXTranslationUnit_CacheCompletionResults : /**
        * Used to indicate that the translation unit should cache some
        * code-completion results with each reparse of the source file.
@@ -5720,15 +6044,15 @@
        * Caching of code-completion results is a performance optimization that
        * introduces some overhead to reparsing but improves the performance of
        * code-completion operations.
        */
     
       CXTranslationUnit_ForSerialization : /**
        * Used to indicate that the translation unit will be serialized with
-       * \c clang_saveTranslationUnit.
+       * \\c clang_saveTranslationUnit.
        *
        * This option is typically used when parsing a header with the intent of
        * producing a precompiled header.
        */
     
       CXTranslationUnit_CXXChainedPCH : /**
        * DEPRECATED: Enabled chained precompiled preambles in C++.
@@ -6119,27 +6443,35 @@
     
       CXType_OCLIntelSubgroupAVCImeResult : /* OpenCL builtin types. */
     
       CXType_OCLIntelSubgroupAVCRefResult : /* OpenCL builtin types. */
     
       CXType_OCLIntelSubgroupAVCSicResult : /* OpenCL builtin types. */
     
-      CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout : /* OpenCL builtin types. */
+      CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout : /* OpenCL builtin types. */
+    
+      CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout : /* OpenCL builtin types. */
+    
+      CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin : /* OpenCL builtin types. */
+    
+      CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin : /* OpenCL builtin types. */
+    
+      CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout : /* OpenCL builtin types. */
+      CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_OCLIntelSubgroupAVCImeSingleRefStreamin : /* OpenCL builtin types. */
+      CXType_OCLIntelSubgroupAVCImeSingleRefStreamin : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_OCLIntelSubgroupAVCImeDualRefStreamin : /* OpenCL builtin types. */
+      CXType_OCLIntelSubgroupAVCImeDualRefStreamin : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_ExtVector : /* OpenCL builtin types. */
+      CXType_ExtVector : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_Atomic : /* OpenCL builtin types. */
+      CXType_Atomic : /* Old aliases for AVC OpenCL extension types. */
     
-      CXType_BTFTagAttributed : /* OpenCL builtin types. */
+      CXType_BTFTagAttributed : /* Old aliases for AVC OpenCL extension types. */
     """
     CXType_Accum: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Accum: 34>
     CXType_Atomic: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Atomic: 177>
     CXType_Attributed: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Attributed: 163>
     CXType_Auto: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Auto: 118>
     CXType_BFloat16: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_BFloat16: 39>
     CXType_BTFTagAttributed: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_BTFTagAttributed: 178>
@@ -6210,20 +6542,24 @@
     CXType_OCLImage2dMSAAWO: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage2dMSAAWO: 140>
     CXType_OCLImage2dRO: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage2dRO: 124>
     CXType_OCLImage2dRW: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage2dRW: 148>
     CXType_OCLImage2dWO: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage2dWO: 136>
     CXType_OCLImage3dRO: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage3dRO: 132>
     CXType_OCLImage3dRW: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage3dRW: 156>
     CXType_OCLImage3dWO: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLImage3dWO: 144>
-    CXType_OCLIntelSubgroupAVCImeDualRefStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualRefStreamin: 175>
+    CXType_OCLIntelSubgroupAVCImeDualRefStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin: 175>
+    CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin: 175>
     CXType_OCLIntelSubgroupAVCImePayload: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImePayload: 165>
     CXType_OCLIntelSubgroupAVCImeResult: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResult: 169>
-    CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout: 173>
-    CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout: 172>
-    CXType_OCLIntelSubgroupAVCImeSingleRefStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleRefStreamin: 174>
+    CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout: 173>
+    CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout: 173>
+    CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout: 172>
+    CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout: 172>
+    CXType_OCLIntelSubgroupAVCImeSingleRefStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin: 174>
+    CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin: 174>
     CXType_OCLIntelSubgroupAVCMcePayload: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCMcePayload: 164>
     CXType_OCLIntelSubgroupAVCMceResult: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCMceResult: 168>
     CXType_OCLIntelSubgroupAVCRefPayload: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCRefPayload: 166>
     CXType_OCLIntelSubgroupAVCRefResult: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCRefResult: 170>
     CXType_OCLIntelSubgroupAVCSicPayload: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCSicPayload: 167>
     CXType_OCLIntelSubgroupAVCSicResult: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLIntelSubgroupAVCSicResult: 171>
     CXType_OCLQueue: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_OCLQueue: 159>
@@ -6255,15 +6591,15 @@
     CXType_UShort: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_UShort: 8>
     CXType_UShortAccum: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_UShortAccum: 36>
     CXType_Unexposed: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Unexposed: 1>
     CXType_VariableArray: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_VariableArray: 115>
     CXType_Vector: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Vector: 113>
     CXType_Void: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_Void: 2>
     CXType_WChar: typing.ClassVar[CXTypeKind]  # value = <CXTypeKind.CXType_WChar: 15>
-    __members__: typing.ClassVar[dict[str, CXTypeKind]]  # value = {'CXType_Invalid': <CXTypeKind.CXType_Invalid: 0>, 'CXType_Unexposed': <CXTypeKind.CXType_Unexposed: 1>, 'CXType_Void': <CXTypeKind.CXType_Void: 2>, 'CXType_Bool': <CXTypeKind.CXType_Bool: 3>, 'CXType_Char_U': <CXTypeKind.CXType_Char_U: 4>, 'CXType_UChar': <CXTypeKind.CXType_UChar: 5>, 'CXType_Char16': <CXTypeKind.CXType_Char16: 6>, 'CXType_Char32': <CXTypeKind.CXType_Char32: 7>, 'CXType_UShort': <CXTypeKind.CXType_UShort: 8>, 'CXType_UInt': <CXTypeKind.CXType_UInt: 9>, 'CXType_ULong': <CXTypeKind.CXType_ULong: 10>, 'CXType_ULongLong': <CXTypeKind.CXType_ULongLong: 11>, 'CXType_UInt128': <CXTypeKind.CXType_UInt128: 12>, 'CXType_Char_S': <CXTypeKind.CXType_Char_S: 13>, 'CXType_SChar': <CXTypeKind.CXType_SChar: 14>, 'CXType_WChar': <CXTypeKind.CXType_WChar: 15>, 'CXType_Short': <CXTypeKind.CXType_Short: 16>, 'CXType_Int': <CXTypeKind.CXType_Int: 17>, 'CXType_Long': <CXTypeKind.CXType_Long: 18>, 'CXType_LongLong': <CXTypeKind.CXType_LongLong: 19>, 'CXType_Int128': <CXTypeKind.CXType_Int128: 20>, 'CXType_Float': <CXTypeKind.CXType_Float: 21>, 'CXType_Double': <CXTypeKind.CXType_Double: 22>, 'CXType_LongDouble': <CXTypeKind.CXType_LongDouble: 23>, 'CXType_NullPtr': <CXTypeKind.CXType_NullPtr: 24>, 'CXType_Overload': <CXTypeKind.CXType_Overload: 25>, 'CXType_Dependent': <CXTypeKind.CXType_Dependent: 26>, 'CXType_ObjCId': <CXTypeKind.CXType_ObjCId: 27>, 'CXType_ObjCClass': <CXTypeKind.CXType_ObjCClass: 28>, 'CXType_ObjCSel': <CXTypeKind.CXType_ObjCSel: 29>, 'CXType_Float128': <CXTypeKind.CXType_Float128: 30>, 'CXType_Half': <CXTypeKind.CXType_Half: 31>, 'CXType_Float16': <CXTypeKind.CXType_Float16: 32>, 'CXType_ShortAccum': <CXTypeKind.CXType_ShortAccum: 33>, 'CXType_Accum': <CXTypeKind.CXType_Accum: 34>, 'CXType_LongAccum': <CXTypeKind.CXType_LongAccum: 35>, 'CXType_UShortAccum': <CXTypeKind.CXType_UShortAccum: 36>, 'CXType_UAccum': <CXTypeKind.CXType_UAccum: 37>, 'CXType_ULongAccum': <CXTypeKind.CXType_ULongAccum: 38>, 'CXType_BFloat16': <CXTypeKind.CXType_BFloat16: 39>, 'CXType_Ibm128': <CXTypeKind.CXType_Ibm128: 40>, 'CXType_FirstBuiltin': <CXTypeKind.CXType_Void: 2>, 'CXType_LastBuiltin': <CXTypeKind.CXType_Ibm128: 40>, 'CXType_Complex': <CXTypeKind.CXType_Complex: 100>, 'CXType_Pointer': <CXTypeKind.CXType_Pointer: 101>, 'CXType_BlockPointer': <CXTypeKind.CXType_BlockPointer: 102>, 'CXType_LValueReference': <CXTypeKind.CXType_LValueReference: 103>, 'CXType_RValueReference': <CXTypeKind.CXType_RValueReference: 104>, 'CXType_Record': <CXTypeKind.CXType_Record: 105>, 'CXType_Enum': <CXTypeKind.CXType_Enum: 106>, 'CXType_Typedef': <CXTypeKind.CXType_Typedef: 107>, 'CXType_ObjCInterface': <CXTypeKind.CXType_ObjCInterface: 108>, 'CXType_ObjCObjectPointer': <CXTypeKind.CXType_ObjCObjectPointer: 109>, 'CXType_FunctionNoProto': <CXTypeKind.CXType_FunctionNoProto: 110>, 'CXType_FunctionProto': <CXTypeKind.CXType_FunctionProto: 111>, 'CXType_ConstantArray': <CXTypeKind.CXType_ConstantArray: 112>, 'CXType_Vector': <CXTypeKind.CXType_Vector: 113>, 'CXType_IncompleteArray': <CXTypeKind.CXType_IncompleteArray: 114>, 'CXType_VariableArray': <CXTypeKind.CXType_VariableArray: 115>, 'CXType_DependentSizedArray': <CXTypeKind.CXType_DependentSizedArray: 116>, 'CXType_MemberPointer': <CXTypeKind.CXType_MemberPointer: 117>, 'CXType_Auto': <CXTypeKind.CXType_Auto: 118>, 'CXType_Elaborated': <CXTypeKind.CXType_Elaborated: 119>, 'CXType_Pipe': <CXTypeKind.CXType_Pipe: 120>, 'CXType_OCLImage1dRO': <CXTypeKind.CXType_OCLImage1dRO: 121>, 'CXType_OCLImage1dArrayRO': <CXTypeKind.CXType_OCLImage1dArrayRO: 122>, 'CXType_OCLImage1dBufferRO': <CXTypeKind.CXType_OCLImage1dBufferRO: 123>, 'CXType_OCLImage2dRO': <CXTypeKind.CXType_OCLImage2dRO: 124>, 'CXType_OCLImage2dArrayRO': <CXTypeKind.CXType_OCLImage2dArrayRO: 125>, 'CXType_OCLImage2dDepthRO': <CXTypeKind.CXType_OCLImage2dDepthRO: 126>, 'CXType_OCLImage2dArrayDepthRO': <CXTypeKind.CXType_OCLImage2dArrayDepthRO: 127>, 'CXType_OCLImage2dMSAARO': <CXTypeKind.CXType_OCLImage2dMSAARO: 128>, 'CXType_OCLImage2dArrayMSAARO': <CXTypeKind.CXType_OCLImage2dArrayMSAARO: 129>, 'CXType_OCLImage2dMSAADepthRO': <CXTypeKind.CXType_OCLImage2dMSAADepthRO: 130>, 'CXType_OCLImage2dArrayMSAADepthRO': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthRO: 131>, 'CXType_OCLImage3dRO': <CXTypeKind.CXType_OCLImage3dRO: 132>, 'CXType_OCLImage1dWO': <CXTypeKind.CXType_OCLImage1dWO: 133>, 'CXType_OCLImage1dArrayWO': <CXTypeKind.CXType_OCLImage1dArrayWO: 134>, 'CXType_OCLImage1dBufferWO': <CXTypeKind.CXType_OCLImage1dBufferWO: 135>, 'CXType_OCLImage2dWO': <CXTypeKind.CXType_OCLImage2dWO: 136>, 'CXType_OCLImage2dArrayWO': <CXTypeKind.CXType_OCLImage2dArrayWO: 137>, 'CXType_OCLImage2dDepthWO': <CXTypeKind.CXType_OCLImage2dDepthWO: 138>, 'CXType_OCLImage2dArrayDepthWO': <CXTypeKind.CXType_OCLImage2dArrayDepthWO: 139>, 'CXType_OCLImage2dMSAAWO': <CXTypeKind.CXType_OCLImage2dMSAAWO: 140>, 'CXType_OCLImage2dArrayMSAAWO': <CXTypeKind.CXType_OCLImage2dArrayMSAAWO: 141>, 'CXType_OCLImage2dMSAADepthWO': <CXTypeKind.CXType_OCLImage2dMSAADepthWO: 142>, 'CXType_OCLImage2dArrayMSAADepthWO': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthWO: 143>, 'CXType_OCLImage3dWO': <CXTypeKind.CXType_OCLImage3dWO: 144>, 'CXType_OCLImage1dRW': <CXTypeKind.CXType_OCLImage1dRW: 145>, 'CXType_OCLImage1dArrayRW': <CXTypeKind.CXType_OCLImage1dArrayRW: 146>, 'CXType_OCLImage1dBufferRW': <CXTypeKind.CXType_OCLImage1dBufferRW: 147>, 'CXType_OCLImage2dRW': <CXTypeKind.CXType_OCLImage2dRW: 148>, 'CXType_OCLImage2dArrayRW': <CXTypeKind.CXType_OCLImage2dArrayRW: 149>, 'CXType_OCLImage2dDepthRW': <CXTypeKind.CXType_OCLImage2dDepthRW: 150>, 'CXType_OCLImage2dArrayDepthRW': <CXTypeKind.CXType_OCLImage2dArrayDepthRW: 151>, 'CXType_OCLImage2dMSAARW': <CXTypeKind.CXType_OCLImage2dMSAARW: 152>, 'CXType_OCLImage2dArrayMSAARW': <CXTypeKind.CXType_OCLImage2dArrayMSAARW: 153>, 'CXType_OCLImage2dMSAADepthRW': <CXTypeKind.CXType_OCLImage2dMSAADepthRW: 154>, 'CXType_OCLImage2dArrayMSAADepthRW': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthRW: 155>, 'CXType_OCLImage3dRW': <CXTypeKind.CXType_OCLImage3dRW: 156>, 'CXType_OCLSampler': <CXTypeKind.CXType_OCLSampler: 157>, 'CXType_OCLEvent': <CXTypeKind.CXType_OCLEvent: 158>, 'CXType_OCLQueue': <CXTypeKind.CXType_OCLQueue: 159>, 'CXType_OCLReserveID': <CXTypeKind.CXType_OCLReserveID: 160>, 'CXType_ObjCObject': <CXTypeKind.CXType_ObjCObject: 161>, 'CXType_ObjCTypeParam': <CXTypeKind.CXType_ObjCTypeParam: 162>, 'CXType_Attributed': <CXTypeKind.CXType_Attributed: 163>, 'CXType_OCLIntelSubgroupAVCMcePayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCMcePayload: 164>, 'CXType_OCLIntelSubgroupAVCImePayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCImePayload: 165>, 'CXType_OCLIntelSubgroupAVCRefPayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCRefPayload: 166>, 'CXType_OCLIntelSubgroupAVCSicPayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCSicPayload: 167>, 'CXType_OCLIntelSubgroupAVCMceResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCMceResult: 168>, 'CXType_OCLIntelSubgroupAVCImeResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResult: 169>, 'CXType_OCLIntelSubgroupAVCRefResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCRefResult: 170>, 'CXType_OCLIntelSubgroupAVCSicResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCSicResult: 171>, 'CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout: 172>, 'CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout: 173>, 'CXType_OCLIntelSubgroupAVCImeSingleRefStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleRefStreamin: 174>, 'CXType_OCLIntelSubgroupAVCImeDualRefStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualRefStreamin: 175>, 'CXType_ExtVector': <CXTypeKind.CXType_ExtVector: 176>, 'CXType_Atomic': <CXTypeKind.CXType_Atomic: 177>, 'CXType_BTFTagAttributed': <CXTypeKind.CXType_BTFTagAttributed: 178>}
+    __members__: typing.ClassVar[dict[str, CXTypeKind]]  # value = {'CXType_Invalid': <CXTypeKind.CXType_Invalid: 0>, 'CXType_Unexposed': <CXTypeKind.CXType_Unexposed: 1>, 'CXType_Void': <CXTypeKind.CXType_Void: 2>, 'CXType_Bool': <CXTypeKind.CXType_Bool: 3>, 'CXType_Char_U': <CXTypeKind.CXType_Char_U: 4>, 'CXType_UChar': <CXTypeKind.CXType_UChar: 5>, 'CXType_Char16': <CXTypeKind.CXType_Char16: 6>, 'CXType_Char32': <CXTypeKind.CXType_Char32: 7>, 'CXType_UShort': <CXTypeKind.CXType_UShort: 8>, 'CXType_UInt': <CXTypeKind.CXType_UInt: 9>, 'CXType_ULong': <CXTypeKind.CXType_ULong: 10>, 'CXType_ULongLong': <CXTypeKind.CXType_ULongLong: 11>, 'CXType_UInt128': <CXTypeKind.CXType_UInt128: 12>, 'CXType_Char_S': <CXTypeKind.CXType_Char_S: 13>, 'CXType_SChar': <CXTypeKind.CXType_SChar: 14>, 'CXType_WChar': <CXTypeKind.CXType_WChar: 15>, 'CXType_Short': <CXTypeKind.CXType_Short: 16>, 'CXType_Int': <CXTypeKind.CXType_Int: 17>, 'CXType_Long': <CXTypeKind.CXType_Long: 18>, 'CXType_LongLong': <CXTypeKind.CXType_LongLong: 19>, 'CXType_Int128': <CXTypeKind.CXType_Int128: 20>, 'CXType_Float': <CXTypeKind.CXType_Float: 21>, 'CXType_Double': <CXTypeKind.CXType_Double: 22>, 'CXType_LongDouble': <CXTypeKind.CXType_LongDouble: 23>, 'CXType_NullPtr': <CXTypeKind.CXType_NullPtr: 24>, 'CXType_Overload': <CXTypeKind.CXType_Overload: 25>, 'CXType_Dependent': <CXTypeKind.CXType_Dependent: 26>, 'CXType_ObjCId': <CXTypeKind.CXType_ObjCId: 27>, 'CXType_ObjCClass': <CXTypeKind.CXType_ObjCClass: 28>, 'CXType_ObjCSel': <CXTypeKind.CXType_ObjCSel: 29>, 'CXType_Float128': <CXTypeKind.CXType_Float128: 30>, 'CXType_Half': <CXTypeKind.CXType_Half: 31>, 'CXType_Float16': <CXTypeKind.CXType_Float16: 32>, 'CXType_ShortAccum': <CXTypeKind.CXType_ShortAccum: 33>, 'CXType_Accum': <CXTypeKind.CXType_Accum: 34>, 'CXType_LongAccum': <CXTypeKind.CXType_LongAccum: 35>, 'CXType_UShortAccum': <CXTypeKind.CXType_UShortAccum: 36>, 'CXType_UAccum': <CXTypeKind.CXType_UAccum: 37>, 'CXType_ULongAccum': <CXTypeKind.CXType_ULongAccum: 38>, 'CXType_BFloat16': <CXTypeKind.CXType_BFloat16: 39>, 'CXType_Ibm128': <CXTypeKind.CXType_Ibm128: 40>, 'CXType_FirstBuiltin': <CXTypeKind.CXType_Void: 2>, 'CXType_LastBuiltin': <CXTypeKind.CXType_Ibm128: 40>, 'CXType_Complex': <CXTypeKind.CXType_Complex: 100>, 'CXType_Pointer': <CXTypeKind.CXType_Pointer: 101>, 'CXType_BlockPointer': <CXTypeKind.CXType_BlockPointer: 102>, 'CXType_LValueReference': <CXTypeKind.CXType_LValueReference: 103>, 'CXType_RValueReference': <CXTypeKind.CXType_RValueReference: 104>, 'CXType_Record': <CXTypeKind.CXType_Record: 105>, 'CXType_Enum': <CXTypeKind.CXType_Enum: 106>, 'CXType_Typedef': <CXTypeKind.CXType_Typedef: 107>, 'CXType_ObjCInterface': <CXTypeKind.CXType_ObjCInterface: 108>, 'CXType_ObjCObjectPointer': <CXTypeKind.CXType_ObjCObjectPointer: 109>, 'CXType_FunctionNoProto': <CXTypeKind.CXType_FunctionNoProto: 110>, 'CXType_FunctionProto': <CXTypeKind.CXType_FunctionProto: 111>, 'CXType_ConstantArray': <CXTypeKind.CXType_ConstantArray: 112>, 'CXType_Vector': <CXTypeKind.CXType_Vector: 113>, 'CXType_IncompleteArray': <CXTypeKind.CXType_IncompleteArray: 114>, 'CXType_VariableArray': <CXTypeKind.CXType_VariableArray: 115>, 'CXType_DependentSizedArray': <CXTypeKind.CXType_DependentSizedArray: 116>, 'CXType_MemberPointer': <CXTypeKind.CXType_MemberPointer: 117>, 'CXType_Auto': <CXTypeKind.CXType_Auto: 118>, 'CXType_Elaborated': <CXTypeKind.CXType_Elaborated: 119>, 'CXType_Pipe': <CXTypeKind.CXType_Pipe: 120>, 'CXType_OCLImage1dRO': <CXTypeKind.CXType_OCLImage1dRO: 121>, 'CXType_OCLImage1dArrayRO': <CXTypeKind.CXType_OCLImage1dArrayRO: 122>, 'CXType_OCLImage1dBufferRO': <CXTypeKind.CXType_OCLImage1dBufferRO: 123>, 'CXType_OCLImage2dRO': <CXTypeKind.CXType_OCLImage2dRO: 124>, 'CXType_OCLImage2dArrayRO': <CXTypeKind.CXType_OCLImage2dArrayRO: 125>, 'CXType_OCLImage2dDepthRO': <CXTypeKind.CXType_OCLImage2dDepthRO: 126>, 'CXType_OCLImage2dArrayDepthRO': <CXTypeKind.CXType_OCLImage2dArrayDepthRO: 127>, 'CXType_OCLImage2dMSAARO': <CXTypeKind.CXType_OCLImage2dMSAARO: 128>, 'CXType_OCLImage2dArrayMSAARO': <CXTypeKind.CXType_OCLImage2dArrayMSAARO: 129>, 'CXType_OCLImage2dMSAADepthRO': <CXTypeKind.CXType_OCLImage2dMSAADepthRO: 130>, 'CXType_OCLImage2dArrayMSAADepthRO': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthRO: 131>, 'CXType_OCLImage3dRO': <CXTypeKind.CXType_OCLImage3dRO: 132>, 'CXType_OCLImage1dWO': <CXTypeKind.CXType_OCLImage1dWO: 133>, 'CXType_OCLImage1dArrayWO': <CXTypeKind.CXType_OCLImage1dArrayWO: 134>, 'CXType_OCLImage1dBufferWO': <CXTypeKind.CXType_OCLImage1dBufferWO: 135>, 'CXType_OCLImage2dWO': <CXTypeKind.CXType_OCLImage2dWO: 136>, 'CXType_OCLImage2dArrayWO': <CXTypeKind.CXType_OCLImage2dArrayWO: 137>, 'CXType_OCLImage2dDepthWO': <CXTypeKind.CXType_OCLImage2dDepthWO: 138>, 'CXType_OCLImage2dArrayDepthWO': <CXTypeKind.CXType_OCLImage2dArrayDepthWO: 139>, 'CXType_OCLImage2dMSAAWO': <CXTypeKind.CXType_OCLImage2dMSAAWO: 140>, 'CXType_OCLImage2dArrayMSAAWO': <CXTypeKind.CXType_OCLImage2dArrayMSAAWO: 141>, 'CXType_OCLImage2dMSAADepthWO': <CXTypeKind.CXType_OCLImage2dMSAADepthWO: 142>, 'CXType_OCLImage2dArrayMSAADepthWO': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthWO: 143>, 'CXType_OCLImage3dWO': <CXTypeKind.CXType_OCLImage3dWO: 144>, 'CXType_OCLImage1dRW': <CXTypeKind.CXType_OCLImage1dRW: 145>, 'CXType_OCLImage1dArrayRW': <CXTypeKind.CXType_OCLImage1dArrayRW: 146>, 'CXType_OCLImage1dBufferRW': <CXTypeKind.CXType_OCLImage1dBufferRW: 147>, 'CXType_OCLImage2dRW': <CXTypeKind.CXType_OCLImage2dRW: 148>, 'CXType_OCLImage2dArrayRW': <CXTypeKind.CXType_OCLImage2dArrayRW: 149>, 'CXType_OCLImage2dDepthRW': <CXTypeKind.CXType_OCLImage2dDepthRW: 150>, 'CXType_OCLImage2dArrayDepthRW': <CXTypeKind.CXType_OCLImage2dArrayDepthRW: 151>, 'CXType_OCLImage2dMSAARW': <CXTypeKind.CXType_OCLImage2dMSAARW: 152>, 'CXType_OCLImage2dArrayMSAARW': <CXTypeKind.CXType_OCLImage2dArrayMSAARW: 153>, 'CXType_OCLImage2dMSAADepthRW': <CXTypeKind.CXType_OCLImage2dMSAADepthRW: 154>, 'CXType_OCLImage2dArrayMSAADepthRW': <CXTypeKind.CXType_OCLImage2dArrayMSAADepthRW: 155>, 'CXType_OCLImage3dRW': <CXTypeKind.CXType_OCLImage3dRW: 156>, 'CXType_OCLSampler': <CXTypeKind.CXType_OCLSampler: 157>, 'CXType_OCLEvent': <CXTypeKind.CXType_OCLEvent: 158>, 'CXType_OCLQueue': <CXTypeKind.CXType_OCLQueue: 159>, 'CXType_OCLReserveID': <CXTypeKind.CXType_OCLReserveID: 160>, 'CXType_ObjCObject': <CXTypeKind.CXType_ObjCObject: 161>, 'CXType_ObjCTypeParam': <CXTypeKind.CXType_ObjCTypeParam: 162>, 'CXType_Attributed': <CXTypeKind.CXType_Attributed: 163>, 'CXType_OCLIntelSubgroupAVCMcePayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCMcePayload: 164>, 'CXType_OCLIntelSubgroupAVCImePayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCImePayload: 165>, 'CXType_OCLIntelSubgroupAVCRefPayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCRefPayload: 166>, 'CXType_OCLIntelSubgroupAVCSicPayload': <CXTypeKind.CXType_OCLIntelSubgroupAVCSicPayload: 167>, 'CXType_OCLIntelSubgroupAVCMceResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCMceResult: 168>, 'CXType_OCLIntelSubgroupAVCImeResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResult: 169>, 'CXType_OCLIntelSubgroupAVCRefResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCRefResult: 170>, 'CXType_OCLIntelSubgroupAVCSicResult': <CXTypeKind.CXType_OCLIntelSubgroupAVCSicResult: 171>, 'CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout: 172>, 'CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout: 173>, 'CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin: 174>, 'CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin: 175>, 'CXType_OCLIntelSubgroupAVCImeResultSingleRefStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultSingleReferenceStreamout: 172>, 'CXType_OCLIntelSubgroupAVCImeResultDualRefStreamout': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeResultDualReferenceStreamout: 173>, 'CXType_OCLIntelSubgroupAVCImeSingleRefStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeSingleReferenceStreamin: 174>, 'CXType_OCLIntelSubgroupAVCImeDualRefStreamin': <CXTypeKind.CXType_OCLIntelSubgroupAVCImeDualReferenceStreamin: 175>, 'CXType_ExtVector': <CXTypeKind.CXType_ExtVector: 176>, 'CXType_Atomic': <CXTypeKind.CXType_Atomic: 177>, 'CXType_BTFTagAttributed': <CXTypeKind.CXType_BTFTagAttributed: 178>}
     def __and__(self, other: typing.Any) -> typing.Any:
         ...
     def __eq__(self, other: typing.Any) -> bool:
         ...
     def __ge__(self, other: typing.Any) -> bool:
         ...
     def __getstate__(self) -> int:
@@ -6307,17 +6643,17 @@
         ...
     @property
     def value(self) -> int:
         ...
 class CXTypeLayoutError:
     """
     /**
-     * List the possible error codes for \c clang_Type_getSizeOf,
-     *   \c clang_Type_getAlignOf, \c clang_Type_getOffsetOf and
-     *   \c clang_Cursor_getOffsetOf.
+     * List the possible error codes for \\c clang_Type_getSizeOf,
+     *   \\c clang_Type_getAlignOf, \\c clang_Type_getOffsetOf and
+     *   \\c clang_Cursor_getOffsetOf.
      *
      * A value of this enumeration type can be returned if the target type is not
      * a valid argument to sizeof, alignof or offsetof.
      */
     
     Members:
     
@@ -6480,14 +6816,116 @@
         ...
     @property
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
+class CXUnaryOperatorKind:
+    """
+    /**
+     * Describes the kind of unary operators.
+     */
+    
+    Members:
+    
+      CXUnaryOperator_Invalid : /** This value describes cursors which are not unary operators. */
+    
+      CXUnaryOperator_PostInc : /** Postfix increment operator. */
+    
+      CXUnaryOperator_PostDec : /** Postfix decrement operator. */
+    
+      CXUnaryOperator_PreInc : /** Prefix increment operator. */
+    
+      CXUnaryOperator_PreDec : /** Prefix decrement operator. */
+    
+      CXUnaryOperator_AddrOf : /** Address of operator. */
+    
+      CXUnaryOperator_Deref : /** Dereference operator. */
+    
+      CXUnaryOperator_Plus : /** Plus operator. */
+    
+      CXUnaryOperator_Minus : /** Minus operator. */
+    
+      CXUnaryOperator_Not : /** Not operator. */
+    
+      CXUnaryOperator_LNot : /** LNot operator. */
+    
+      CXUnaryOperator_Real : /** "__real expr" operator. */
+    
+      CXUnaryOperator_Imag : /** "__imag expr" operator. */
+    
+      CXUnaryOperator_Extension : /** __extension__ marker operator. */
+    
+      CXUnaryOperator_Coawait : /** C++ co_await operator. */
+    """
+    CXUnaryOperator_AddrOf: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_AddrOf: 5>
+    CXUnaryOperator_Coawait: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Coawait: 14>
+    CXUnaryOperator_Deref: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Deref: 6>
+    CXUnaryOperator_Extension: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Extension: 13>
+    CXUnaryOperator_Imag: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Imag: 12>
+    CXUnaryOperator_Invalid: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Invalid: 0>
+    CXUnaryOperator_LNot: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_LNot: 10>
+    CXUnaryOperator_Minus: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Minus: 8>
+    CXUnaryOperator_Not: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Not: 9>
+    CXUnaryOperator_Plus: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Plus: 7>
+    CXUnaryOperator_PostDec: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_PostDec: 2>
+    CXUnaryOperator_PostInc: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_PostInc: 1>
+    CXUnaryOperator_PreDec: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_PreDec: 4>
+    CXUnaryOperator_PreInc: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_PreInc: 3>
+    CXUnaryOperator_Real: typing.ClassVar[CXUnaryOperatorKind]  # value = <CXUnaryOperatorKind.CXUnaryOperator_Real: 11>
+    __members__: typing.ClassVar[dict[str, CXUnaryOperatorKind]]  # value = {'CXUnaryOperator_Invalid': <CXUnaryOperatorKind.CXUnaryOperator_Invalid: 0>, 'CXUnaryOperator_PostInc': <CXUnaryOperatorKind.CXUnaryOperator_PostInc: 1>, 'CXUnaryOperator_PostDec': <CXUnaryOperatorKind.CXUnaryOperator_PostDec: 2>, 'CXUnaryOperator_PreInc': <CXUnaryOperatorKind.CXUnaryOperator_PreInc: 3>, 'CXUnaryOperator_PreDec': <CXUnaryOperatorKind.CXUnaryOperator_PreDec: 4>, 'CXUnaryOperator_AddrOf': <CXUnaryOperatorKind.CXUnaryOperator_AddrOf: 5>, 'CXUnaryOperator_Deref': <CXUnaryOperatorKind.CXUnaryOperator_Deref: 6>, 'CXUnaryOperator_Plus': <CXUnaryOperatorKind.CXUnaryOperator_Plus: 7>, 'CXUnaryOperator_Minus': <CXUnaryOperatorKind.CXUnaryOperator_Minus: 8>, 'CXUnaryOperator_Not': <CXUnaryOperatorKind.CXUnaryOperator_Not: 9>, 'CXUnaryOperator_LNot': <CXUnaryOperatorKind.CXUnaryOperator_LNot: 10>, 'CXUnaryOperator_Real': <CXUnaryOperatorKind.CXUnaryOperator_Real: 11>, 'CXUnaryOperator_Imag': <CXUnaryOperatorKind.CXUnaryOperator_Imag: 12>, 'CXUnaryOperator_Extension': <CXUnaryOperatorKind.CXUnaryOperator_Extension: 13>, 'CXUnaryOperator_Coawait': <CXUnaryOperatorKind.CXUnaryOperator_Coawait: 14>}
+    def __and__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __eq__(self, other: typing.Any) -> bool:
+        ...
+    def __ge__(self, other: typing.Any) -> bool:
+        ...
+    def __getstate__(self) -> int:
+        ...
+    def __gt__(self, other: typing.Any) -> bool:
+        ...
+    def __hash__(self) -> int:
+        ...
+    def __index__(self) -> int:
+        ...
+    def __init__(self, value: int) -> None:
+        ...
+    def __int__(self) -> int:
+        ...
+    def __invert__(self) -> typing.Any:
+        ...
+    def __le__(self, other: typing.Any) -> bool:
+        ...
+    def __lt__(self, other: typing.Any) -> bool:
+        ...
+    def __ne__(self, other: typing.Any) -> bool:
+        ...
+    def __or__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rand__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __repr__(self) -> str:
+        ...
+    def __ror__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __rxor__(self, other: typing.Any) -> typing.Any:
+        ...
+    def __setstate__(self, state: int) -> None:
+        ...
+    def __str__(self) -> str:
+        ...
+    def __xor__(self, other: typing.Any) -> typing.Any:
+        ...
+    @property
+    def name(self) -> str:
+        ...
+    @property
+    def value(self) -> int:
+        ...
 class CXUnsavedFile:
     """
     /**
      * Provides the contents of a file that has not yet been saved to disk.
      *
      * Each CXUnsavedFile instance provides the name of a file on the
      * system along with the current contents of that file that have not
@@ -6645,15 +7083,15 @@
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
 class CXVisitorResult:
     """
-    /** \defgroup CINDEX_HIGH Higher level API functions
+    /** \\defgroup CINDEX_HIGH Higher level API functions
      *
      * @{
      */
     
     Members:
     
       CXVisit_Break
@@ -6882,14 +7320,26 @@
         ...
 class TokenArray:
     def at(self, arg0: int) -> CXToken:
         ...
     @property
     def n(self) -> int:
         ...
+class _CXChildVisitResultp(_PointerWrapperBase):
+    @staticmethod
+    def from_capsule(arg0: capsule) -> _CXChildVisitResultp:
+        ...
+    def __init__(self, arg0: int) -> None:
+        ...
+class _CXCursorAndRangeVisitorBlockp(_PointerWrapperBase):
+    @staticmethod
+    def from_capsule(arg0: capsule) -> _CXCursorAndRangeVisitorBlockp:
+        ...
+    def __init__(self, arg0: int) -> None:
+        ...
 class _PointerWrapperBase:
     @typing.overload
     def __init__(self, arg0: capsule) -> None:
         ...
     @typing.overload
     def __init__(self, arg0: int) -> None:
         ...
@@ -6950,92 +7400,103 @@
     def from_capsule(arg0: capsule) -> voidpp:
         ...
     def __init__(self, arg0: int) -> None:
         ...
 def clang_BlockCommandComment_getArgText(arg0: CXComment, arg1: int) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_BlockCommand AST node.
+     * \\param Comment a \\c CXComment_BlockCommand AST node.
      *
-     * \param ArgIdx argument index (zero-based).
+     * \\param ArgIdx argument index (zero-based).
      *
-     * \returns text of the specified word-like argument.
+     * \\returns text of the specified word-like argument.
      */
     """
 def clang_BlockCommandComment_getCommandName(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_BlockCommand AST node.
+     * \\param Comment a \\c CXComment_BlockCommand AST node.
      *
-     * \returns name of the block command.
+     * \\returns name of the block command.
      */
     """
 def clang_BlockCommandComment_getNumArgs(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_BlockCommand AST node.
+     * \\param Comment a \\c CXComment_BlockCommand AST node.
      *
-     * \returns number of word-like arguments.
+     * \\returns number of word-like arguments.
      */
     """
 def clang_BlockCommandComment_getParagraph(arg0: CXComment) -> CXComment:
     """
     /**
-     * \param Comment a \c CXComment_BlockCommand or
-     * \c CXComment_VerbatimBlockCommand AST node.
+     * \\param Comment a \\c CXComment_BlockCommand or
+     * \\c CXComment_VerbatimBlockCommand AST node.
      *
-     * \returns paragraph argument of the block command.
+     * \\returns paragraph argument of the block command.
      */
     """
 def clang_CXCursorSet_contains(arg0: CXCursorSetImplp, arg1: CXCursor) -> int:
     """
     /**
      * Queries a CXCursorSet to see if it contains a specific CXCursor.
      *
-     * \returns non-zero if the set contains the specified cursor.
+     * \\returns non-zero if the set contains the specified cursor.
      */
     """
 def clang_CXCursorSet_insert(arg0: CXCursorSetImplp, arg1: CXCursor) -> int:
     """
     /**
      * Inserts a CXCursor into a CXCursorSet.
      *
-     * \returns zero if the CXCursor was already in the set, and non-zero otherwise.
+     * \\returns zero if the CXCursor was already in the set, and non-zero otherwise.
      */
     """
 def clang_CXIndex_getGlobalOptions(arg0: voidp) -> int:
     """
     /**
      * Gets the general options associated with a CXIndex.
      *
-     * \returns A bitmask of options, a bitwise OR of CXGlobalOpt_XXX flags that
+     * This function allows to obtain the final option values used by libclang after
+     * specifying the option policies via CXChoice enumerators.
+     *
+     * \\returns A bitmask of options, a bitwise OR of CXGlobalOpt_XXX flags that
      * are associated with the given CXIndex object.
      */
     """
 def clang_CXIndex_setGlobalOptions(arg0: voidp, arg1: int) -> None:
     """
     /**
      * Sets general options associated with a CXIndex.
      *
+     * This function is DEPRECATED. Set
+     * CXIndexOptions::ThreadBackgroundPriorityForIndexing and/or
+     * CXIndexOptions::ThreadBackgroundPriorityForEditing and call
+     * clang_createIndexWithOptions() instead.
+     *
      * For example:
-     * \code
+     * \\code
      * CXIndex idx = ...;
      * clang_CXIndex_setGlobalOptions(idx,
      *     clang_CXIndex_getGlobalOptions(idx) |
      *     CXGlobalOpt_ThreadBackgroundPriorityForIndexing);
-     * \endcode
+     * \\endcode
      *
-     * \param options A bitmask of options, a bitwise OR of CXGlobalOpt_XXX flags.
+     * \\param options A bitmask of options, a bitwise OR of CXGlobalOpt_XXX flags.
      */
     """
 def clang_CXIndex_setInvocationEmissionPathOption(arg0: voidp, arg1: str) -> None:
     """
     /**
      * Sets the invocation emission path option in a CXIndex.
      *
+     * This function is DEPRECATED. Set CXIndexOptions::InvocationEmissionPath and
+     * call clang_createIndexWithOptions() instead.
+     *
      * The invocation emission path specifies a path which will contain log
      * files for certain libclang invocations. A null value (default) implies that
      * libclang invocations are not logged..
      */
     """
 def clang_CXRewriter_create(arg0: CXTranslationUnitImplp) -> voidp:
     """
@@ -7152,14 +7613,60 @@
     """
 def clang_CXXMethod_isDeleted(arg0: CXCursor) -> int:
     """
     /**
      * Determine if a C++ method is declared '= delete'.
      */
     """
+def clang_CXXMethod_isExplicit(arg0: CXCursor) -> int:
+    """
+    /**
+     * Determines if a C++ constructor or conversion function was declared
+     * explicit, returning 1 if such is the case and 0 otherwise.
+     *
+     * Constructors or conversion functions are declared explicit through
+     * the use of the explicit specifier.
+     *
+     * For example, the following constructor and conversion function are
+     * not explicit as they lack the explicit specifier:
+     *
+     *     class Foo {
+     *         Foo();
+     *         operator int();
+     *     };
+     *
+     * While the following constructor and conversion function are
+     * explicit as they are declared with the explicit specifier.
+     *
+     *     class Foo {
+     *         explicit Foo();
+     *         explicit operator int();
+     *     };
+     *
+     * This function will return 0 when given a cursor pointing to one of
+     * the former declarations and it will return 1 for a cursor pointing
+     * to the latter declarations.
+     *
+     * The explicit specifier allows the user to specify a
+     * conditional compile-time expression whose value decides
+     * whether the marked element is explicit or not.
+     *
+     * For example:
+     *
+     *     constexpr bool foo(int i) { return i % 2 == 0; }
+     *
+     *     class Foo {
+     *          explicit(foo(1)) Foo();
+     *          explicit(foo(2)) operator int();
+     *     }
+     *
+     * This function will return 0 for the constructor and 1 for
+     * the conversion function.
+     */
+    """
 def clang_CXXMethod_isMoveAssignmentOperator(arg0: CXCursor) -> int:
     """
     /**
      * Determine if a C++ member function is a move-assignment operator,
      * returning 1 if such is the case and 0 otherwise.
      *
      * > A move-assignment operator `X::operator=` is a non-static,
@@ -7210,47 +7717,47 @@
      * Determine if a C++ record is abstract, i.e. whether a class or struct
      * has a pure virtual member function.
      */
     """
 def clang_Comment_getChild(arg0: CXComment, arg1: int) -> CXComment:
     """
     /**
-     * \param Comment AST node of any kind.
+     * \\param Comment AST node of any kind.
      *
-     * \param ChildIdx child index (zero-based).
+     * \\param ChildIdx child index (zero-based).
      *
-     * \returns the specified child of the AST node.
+     * \\returns the specified child of the AST node.
      */
     """
 def clang_Comment_getKind(arg0: CXComment) -> CXCommentKind:
     """
     /**
-     * \param Comment AST node of any kind.
+     * \\param Comment AST node of any kind.
      *
-     * \returns the type of the AST node.
+     * \\returns the type of the AST node.
      */
     """
 def clang_Comment_getNumChildren(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment AST node of any kind.
+     * \\param Comment AST node of any kind.
      *
-     * \returns number of children of the AST node.
+     * \\returns number of children of the AST node.
      */
     """
 def clang_Comment_isWhitespace(arg0: CXComment) -> int:
     """
     /**
-     * A \c CXComment_Paragraph node is considered whitespace if it contains
-     * only \c CXComment_Text nodes that are empty or whitespace.
+     * A \\c CXComment_Paragraph node is considered whitespace if it contains
+     * only \\c CXComment_Text nodes that are empty or whitespace.
      *
-     * Other AST nodes (except \c CXComment_Paragraph and \c CXComment_Text) are
+     * Other AST nodes (except \\c CXComment_Paragraph and \\c CXComment_Text) are
      * never considered whitespace.
      *
-     * \returns non-zero if \c Comment is whitespace.
+     * \\returns non-zero if \\c Comment is whitespace.
      */
     """
 def clang_CompilationDatabase_dispose(arg0: voidp) -> None:
     """
     /**
      * Free the given compilation database
      */
@@ -7263,15 +7770,15 @@
      * Get all the compile commands in the given compilation database.
      */
     """
 def clang_CompilationDatabase_getCompileCommands(arg0: voidp, arg1: str) -> voidp:
     """
     /**
      * Find the compile commands used for a file. The compile commands
-     * must be freed by \c clang_CompileCommands_dispose.
+     * must be freed by \\c clang_CompileCommands_dispose.
      */
     """
 def clang_CompileCommand_getArg(arg0: voidp, arg1: int) -> CXString:
     """
     /**
      * Get the I'th argument value in the compiler invocations
      *
@@ -7355,15 +7862,15 @@
      * invalid cursor is returned.
      */
     """
 def clang_Cursor_getBriefCommentText(arg0: CXCursor) -> CXString:
     """
     /**
      * Given a cursor that represents a documentable entity (e.g.,
-     * declaration), return the associated \paragraph; otherwise return the
+     * declaration), return the associated \\paragraph; otherwise return the
      * first paragraph.
      */
     """
 def clang_Cursor_getCXXManglings(arg0: CXCursor) -> CXStringSet:
     """
     /**
      * Retrieve the CXStrings representing the mangled symbols of the C++
@@ -7436,17 +7943,17 @@
      */
     """
 def clang_Cursor_getObjCPropertyAttributes(arg0: CXCursor, arg1: int) -> int:
     """
     /**
      * Given a cursor that represents a property declaration, return the
      * associated property attributes. The bits are formed from
-     * \c CXObjCPropertyAttrKind.
+     * \\c CXObjCPropertyAttrKind.
      *
-     * \param reserved Reserved for future use, pass 0.
+     * \\param reserved Reserved for future use, pass 0.
      */
     """
 def clang_Cursor_getObjCPropertyGetterName(arg0: CXCursor) -> CXString:
     """
     /**
      * Given a cursor that represents a property declaration, return the
      * name of the method that implements the getter.
@@ -7464,15 +7971,15 @@
     /**
      * If the cursor points to a selector identifier in an Objective-C
      * method or message expression, this returns the selector index.
      *
      * After getting a cursor with #clang_getCursor, this can be called to
      * determine if the location points to a selector identifier.
      *
-     * \returns The selector index if the cursor is an Objective-C method or message
+     * \\returns The selector index if the cursor is an Objective-C method or message
      * expression and the cursor is pointing to a selector identifier, or -1
      * otherwise.
      */
     """
 def clang_Cursor_getOffsetOfField(arg0: CXCursor) -> int:
     """
     /**
@@ -7490,15 +7997,15 @@
      */
     """
 def clang_Cursor_getParsedComment(arg0: CXCursor) -> CXComment:
     """
     /**
      * Given a cursor that represents a documentable entity (e.g.,
      * declaration), return the associated parsed comment as a
-     * \c CXComment_FullComment AST node.
+     * \\c CXComment_FullComment AST node.
      */
     """
 def clang_Cursor_getRawCommentText(arg0: CXCursor) -> CXString:
     """
     /**
      * Given a cursor that represents a declaration, return the associated
      * comment text, including comment markers.
@@ -7515,18 +8022,18 @@
     """
     /**
      * Retrieve a range for a piece that forms the cursors spelling name.
      * Most of the times there is only one range for the complete spelling but for
      * Objective-C methods and Objective-C message expressions, there are multiple
      * pieces for each selector identifier.
      *
-     * \param pieceIndex the index of the spelling name piece. If this is greater
+     * \\param pieceIndex the index of the spelling name piece. If this is greater
      * than the actual number of pieces, it will return a NULL (invalid) range.
      *
-     * \param options Reserved.
+     * \\param options Reserved.
      */
     """
 def clang_Cursor_getStorageClass(arg0: CXCursor) -> CX_StorageClass:
     """
     /**
      * Returns the storage class for a function or variable declaration.
      *
@@ -7665,16 +8172,15 @@
      * Determine whether the given cursor represents an anonymous record
      * declaration.
      */
     """
 def clang_Cursor_isBitField(arg0: CXCursor) -> int:
     """
     /**
-     * Returns non-zero if the cursor specifies a Record member that is a
-     *   bitfield.
+     * Returns non-zero if the cursor specifies a Record member that is a bit-field.
      */
     """
 def clang_Cursor_isDynamicCall(arg0: CXCursor) -> int:
     """
     /**
      * Given a cursor pointing to a C++ method call or an Objective-C
      * message, returns non-zero if the method/message is "dynamic", meaning:
@@ -7689,21 +8195,21 @@
     """
 def clang_Cursor_isExternalSymbol(arg0: CXCursor, arg1: CXString, arg2: CXString, arg3: int) -> int:
     """
     /**
      * Returns non-zero if the given cursor points to a symbol marked with
      * external_source_symbol attribute.
      *
-     * \param language If non-NULL, and the attribute is present, will be set to
+     * \\param language If non-NULL, and the attribute is present, will be set to
      * the 'language' string from the attribute.
      *
-     * \param definedIn If non-NULL, and the attribute is present, will be set to
+     * \\param definedIn If non-NULL, and the attribute is present, will be set to
      * the 'definedIn' string from the attribute.
      *
-     * \param isGenerated If non-NULL, and the attribute is present, will be set to
+     * \\param isGenerated If non-NULL, and the attribute is present, will be set to
      * non-zero if the 'generated_declaration' is set in the attribute.
      */
     """
 def clang_Cursor_isFunctionInlined(arg0: CXCursor) -> int:
     """
     /**
      * Determine whether a  CXCursor that is a function declaration, is an
@@ -7730,23 +8236,23 @@
      * Determine whether a  CXCursor that is a macro, is
      * function like.
      */
     """
 def clang_Cursor_isNull(arg0: CXCursor) -> int:
     """
     /**
-     * Returns non-zero if \p cursor is null.
+     * Returns non-zero if \\p cursor is null.
      */
     """
 def clang_Cursor_isObjCOptional(arg0: CXCursor) -> int:
     """
     /**
      * Given a cursor that represents an Objective-C method or property
-     * declaration, return non-zero if the declaration was affected by "\@optional".
-     * Returns zero if the cursor is not such a declaration or it is "\@required".
+     * declaration, return non-zero if the declaration was affected by "\\@optional".
+     * Returns zero if the cursor is not such a declaration or it is "\\@required".
      */
     """
 def clang_Cursor_isVariadic(arg0: CXCursor) -> int:
     """
     /**
      * Returns non-zero if the given cursor is a variadic function or method.
      */
@@ -7813,186 +8319,186 @@
      * Returns a non-zero value if the kind is Int and the evaluation
      * result resulted in an unsigned integer.
      */
     """
 def clang_File_isEqual(arg0: voidp, arg1: voidp) -> int:
     """
     /**
-     * Returns non-zero if the \c file1 and \c file2 point to the same file,
+     * Returns non-zero if the \\c file1 and \\c file2 point to the same file,
      * or they are both NULL.
      */
     """
 def clang_File_tryGetRealPathName(arg0: voidp) -> CXString:
     """
     /**
-     * Returns the real path name of \c file.
+     * Returns the real path name of \\c file.
      *
-     * An empty string may be returned. Use \c clang_getFileName() in that case.
+     * An empty string may be returned. Use \\c clang_getFileName() in that case.
      */
     """
 def clang_FullComment_getAsHTML(arg0: CXComment) -> CXString:
     """
     /**
      * Convert a given full parsed comment to an HTML fragment.
      *
      * Specific details of HTML layout are subject to change.  Don't try to parse
      * this HTML back into an AST, use other APIs instead.
      *
      * Currently the following CSS classes are used:
-     * \li "para-brief" for \paragraph and equivalent commands;
-     * \li "para-returns" for \\returns paragraph and equivalent commands;
-     * \li "word-returns" for the "Returns" word in \\returns paragraph.
+     * \\li "para-brief" for \\paragraph and equivalent commands;
+     * \\li "para-returns" for \\\\returns paragraph and equivalent commands;
+     * \\li "word-returns" for the "Returns" word in \\\\returns paragraph.
      *
-     * Function argument documentation is rendered as a \<dl\> list with arguments
+     * Function argument documentation is rendered as a \\<dl\\> list with arguments
      * sorted in function prototype order.  CSS classes used:
-     * \li "param-name-index-NUMBER" for parameter name (\<dt\>);
-     * \li "param-descr-index-NUMBER" for parameter description (\<dd\>);
-     * \li "param-name-index-invalid" and "param-descr-index-invalid" are used if
+     * \\li "param-name-index-NUMBER" for parameter name (\\<dt\\>);
+     * \\li "param-descr-index-NUMBER" for parameter description (\\<dd\\>);
+     * \\li "param-name-index-invalid" and "param-descr-index-invalid" are used if
      * parameter index is invalid.
      *
-     * Template parameter documentation is rendered as a \<dl\> list with
+     * Template parameter documentation is rendered as a \\<dl\\> list with
      * parameters sorted in template parameter list order.  CSS classes used:
-     * \li "tparam-name-index-NUMBER" for parameter name (\<dt\>);
-     * \li "tparam-descr-index-NUMBER" for parameter description (\<dd\>);
-     * \li "tparam-name-index-other" and "tparam-descr-index-other" are used for
+     * \\li "tparam-name-index-NUMBER" for parameter name (\\<dt\\>);
+     * \\li "tparam-descr-index-NUMBER" for parameter description (\\<dd\\>);
+     * \\li "tparam-name-index-other" and "tparam-descr-index-other" are used for
      * names inside template template parameters;
-     * \li "tparam-name-index-invalid" and "tparam-descr-index-invalid" are used if
+     * \\li "tparam-name-index-invalid" and "tparam-descr-index-invalid" are used if
      * parameter position is invalid.
      *
-     * \param Comment a \c CXComment_FullComment AST node.
+     * \\param Comment a \\c CXComment_FullComment AST node.
      *
-     * \returns string containing an HTML fragment.
+     * \\returns string containing an HTML fragment.
      */
     """
 def clang_FullComment_getAsXML(arg0: CXComment) -> CXString:
     """
     /**
      * Convert a given full parsed comment to an XML document.
      *
      * A Relax NG schema for the XML can be found in comment-xml-schema.rng file
      * inside clang source tree.
      *
-     * \param Comment a \c CXComment_FullComment AST node.
+     * \\param Comment a \\c CXComment_FullComment AST node.
      *
-     * \returns string containing an XML document.
+     * \\returns string containing an XML document.
      */
     """
 def clang_HTMLStartTagComment_isSelfClosing(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_HTMLStartTag AST node.
+     * \\param Comment a \\c CXComment_HTMLStartTag AST node.
      *
-     * \returns non-zero if tag is self-closing (for example, &lt;br /&gt;).
+     * \\returns non-zero if tag is self-closing (for example, &lt;br /&gt;).
      */
     """
 def clang_HTMLStartTag_getAttrName(arg0: CXComment, arg1: int) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_HTMLStartTag AST node.
+     * \\param Comment a \\c CXComment_HTMLStartTag AST node.
      *
-     * \param AttrIdx attribute index (zero-based).
+     * \\param AttrIdx attribute index (zero-based).
      *
-     * \returns name of the specified attribute.
+     * \\returns name of the specified attribute.
      */
     """
 def clang_HTMLStartTag_getAttrValue(arg0: CXComment, arg1: int) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_HTMLStartTag AST node.
+     * \\param Comment a \\c CXComment_HTMLStartTag AST node.
      *
-     * \param AttrIdx attribute index (zero-based).
+     * \\param AttrIdx attribute index (zero-based).
      *
-     * \returns value of the specified attribute.
+     * \\returns value of the specified attribute.
      */
     """
 def clang_HTMLStartTag_getNumAttrs(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_HTMLStartTag AST node.
+     * \\param Comment a \\c CXComment_HTMLStartTag AST node.
      *
-     * \returns number of attributes (name-value pairs) attached to the start tag.
+     * \\returns number of attributes (name-value pairs) attached to the start tag.
      */
     """
 def clang_HTMLTagComment_getAsString(arg0: CXComment) -> CXString:
     """
     /**
      * Convert an HTML tag AST node to string.
      *
-     * \param Comment a \c CXComment_HTMLStartTag or \c CXComment_HTMLEndTag AST
+     * \\param Comment a \\c CXComment_HTMLStartTag or \\c CXComment_HTMLEndTag AST
      * node.
      *
-     * \returns string containing an HTML tag.
+     * \\returns string containing an HTML tag.
      */
     """
 def clang_HTMLTagComment_getTagName(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_HTMLStartTag or \c CXComment_HTMLEndTag AST
+     * \\param Comment a \\c CXComment_HTMLStartTag or \\c CXComment_HTMLEndTag AST
      * node.
      *
-     * \returns HTML tag name.
+     * \\returns HTML tag name.
      */
     """
 def clang_IndexAction_create(arg0: voidp) -> voidp:
     """
     /**
      * An indexing action/session, to be applied to one or multiple
      * translation units.
      *
-     * \param CIdx The index object with which the index action will be associated.
+     * \\param CIdx The index object with which the index action will be associated.
      */
     """
 def clang_IndexAction_dispose(arg0: voidp) -> None:
     """
     /**
      * Destroy the given index action.
      *
      * The index action must not be destroyed until all of the translation units
      * created within that index action have been destroyed.
      */
     """
 def clang_InlineCommandComment_getArgText(arg0: CXComment, arg1: int) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_InlineCommand AST node.
+     * \\param Comment a \\c CXComment_InlineCommand AST node.
      *
-     * \param ArgIdx argument index (zero-based).
+     * \\param ArgIdx argument index (zero-based).
      *
-     * \returns text of the specified argument.
+     * \\returns text of the specified argument.
      */
     """
 def clang_InlineCommandComment_getCommandName(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_InlineCommand AST node.
+     * \\param Comment a \\c CXComment_InlineCommand AST node.
      *
-     * \returns name of the inline command.
+     * \\returns name of the inline command.
      */
     """
 def clang_InlineCommandComment_getNumArgs(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_InlineCommand AST node.
+     * \\param Comment a \\c CXComment_InlineCommand AST node.
      *
-     * \returns number of command arguments.
+     * \\returns number of command arguments.
      */
     """
 def clang_InlineCommandComment_getRenderKind(arg0: CXComment) -> CXCommentInlineCommandRenderKind:
     """
     /**
-     * \param Comment a \c CXComment_InlineCommand AST node.
+     * \\param Comment a \\c CXComment_InlineCommand AST node.
      *
-     * \returns the most appropriate rendering mode, chosen on command
+     * \\returns the most appropriate rendering mode, chosen on command
      * semantics in Doxygen.
      */
     """
 def clang_InlineContentComment_hasTrailingNewline(arg0: CXComment) -> int:
     """
     /**
-     * \returns non-zero if \c Comment is inline content and has a newline
+     * \\returns non-zero if \\c Comment is inline content and has a newline
      * immediately following it in the comment text.  Newlines between paragraphs
      * do not count.
      */
     """
 def clang_Location_isFromMainFile(arg0: CXSourceLocation) -> int:
     """
     /**
@@ -8005,152 +8511,152 @@
     /**
      * Returns non-zero if the given source location is in a system header.
      */
     """
 def clang_ModuleMapDescriptor_create(arg0: int) -> CXModuleMapDescriptorImplp:
     """
     /**
-     * Create a \c CXModuleMapDescriptor object.
-     * Must be disposed with \c clang_ModuleMapDescriptor_dispose().
+     * Create a \\c CXModuleMapDescriptor object.
+     * Must be disposed with \\c clang_ModuleMapDescriptor_dispose().
      *
-     * \param options is reserved, always pass 0.
+     * \\param options is reserved, always pass 0.
      */
     """
 def clang_ModuleMapDescriptor_dispose(arg0: CXModuleMapDescriptorImplp) -> None:
     """
     /**
-     * Dispose a \c CXModuleMapDescriptor object.
+     * Dispose a \\c CXModuleMapDescriptor object.
      */
     """
 def clang_ModuleMapDescriptor_setFrameworkModuleName(arg0: CXModuleMapDescriptorImplp, arg1: str) -> CXErrorCode:
     """
     /**
-     * Sets the framework module name that the module.map describes.
-     * \returns 0 for success, non-zero to indicate an error.
+     * Sets the framework module name that the module.modulemap describes.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_ModuleMapDescriptor_setUmbrellaHeader(arg0: CXModuleMapDescriptorImplp, arg1: str) -> CXErrorCode:
     """
     /**
-     * Sets the umbrella header name that the module.map describes.
-     * \returns 0 for success, non-zero to indicate an error.
+     * Sets the umbrella header name that the module.modulemap describes.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_ModuleMapDescriptor_writeToBuffer(arg0: CXModuleMapDescriptorImplp, arg1: int, arg2: charpp, arg3: int) -> CXErrorCode:
     """
     /**
-     * Write out the \c CXModuleMapDescriptor object to a char buffer.
+     * Write out the \\c CXModuleMapDescriptor object to a char buffer.
      *
-     * \param options is reserved, always pass 0.
-     * \param out_buffer_ptr pointer to receive the buffer pointer, which should be
-     * disposed using \c clang_free().
-     * \param out_buffer_size pointer to receive the buffer size.
-     * \returns 0 for success, non-zero to indicate an error.
+     * \\param options is reserved, always pass 0.
+     * \\param out_buffer_ptr pointer to receive the buffer pointer, which should be
+     * disposed using \\c clang_free().
+     * \\param out_buffer_size pointer to receive the buffer size.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_Module_getASTFile(arg0: voidp) -> voidp:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns the module file where the provided module object came from.
+     * \\returns the module file where the provided module object came from.
      */
     """
 def clang_Module_getFullName(arg0: voidp) -> CXString:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns the full name of the module, e.g. "std.vector".
+     * \\returns the full name of the module, e.g. "std.vector".
      */
     """
 def clang_Module_getName(arg0: voidp) -> CXString:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns the name of the module, e.g. for the 'std.vector' sub-module it
+     * \\returns the name of the module, e.g. for the 'std.vector' sub-module it
      * will return "vector".
      */
     """
 def clang_Module_getNumTopLevelHeaders(arg0: CXTranslationUnitImplp, arg1: voidp) -> int:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns the number of top level headers associated with this module.
+     * \\returns the number of top level headers associated with this module.
      */
     """
 def clang_Module_getParent(arg0: voidp) -> voidp:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns the parent of a sub-module or NULL if the given module is top-level,
+     * \\returns the parent of a sub-module or NULL if the given module is top-level,
      * e.g. for 'std.vector' it will return the 'std' module.
      */
     """
 def clang_Module_getTopLevelHeader(arg0: CXTranslationUnitImplp, arg1: voidp, arg2: int) -> voidp:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \param Index top level header index (zero-based).
+     * \\param Index top level header index (zero-based).
      *
-     * \returns the specified top level header associated with the module.
+     * \\returns the specified top level header associated with the module.
      */
     """
 def clang_Module_isSystem(arg0: voidp) -> int:
     """
     /**
-     * \param Module a module object.
+     * \\param Module a module object.
      *
-     * \returns non-zero if the module is a system one.
+     * \\returns non-zero if the module is a system one.
      */
     """
 def clang_ParamCommandComment_getDirection(arg0: CXComment) -> CXCommentParamPassDirection:
     """
     /**
-     * \param Comment a \c CXComment_ParamCommand AST node.
+     * \\param Comment a \\c CXComment_ParamCommand AST node.
      *
-     * \returns parameter passing direction.
+     * \\returns parameter passing direction.
      */
     """
 def clang_ParamCommandComment_getParamIndex(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_ParamCommand AST node.
+     * \\param Comment a \\c CXComment_ParamCommand AST node.
      *
-     * \returns zero-based parameter index in function prototype.
+     * \\returns zero-based parameter index in function prototype.
      */
     """
 def clang_ParamCommandComment_getParamName(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_ParamCommand AST node.
+     * \\param Comment a \\c CXComment_ParamCommand AST node.
      *
-     * \returns parameter name.
+     * \\returns parameter name.
      */
     """
 def clang_ParamCommandComment_isDirectionExplicit(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_ParamCommand AST node.
+     * \\param Comment a \\c CXComment_ParamCommand AST node.
      *
-     * \returns non-zero if parameter passing direction was specified explicitly in
+     * \\returns non-zero if parameter passing direction was specified explicitly in
      * the comment.
      */
     """
 def clang_ParamCommandComment_isParamIndexValid(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_ParamCommand AST node.
+     * \\param Comment a \\c CXComment_ParamCommand AST node.
      *
-     * \returns non-zero if the parameter that this AST node represents was found
-     * in the function prototype and \c clang_ParamCommandComment_getParamIndex
+     * \\returns non-zero if the parameter that this AST node represents was found
+     * in the function prototype and \\c clang_ParamCommandComment_getParamIndex
      * function will return a meaningful value.
      */
     """
 def clang_PrintingPolicy_dispose(arg0: voidp) -> None:
     """
     /**
      * Release a printing policy.
@@ -8167,71 +8673,71 @@
     /**
      * Set a property value for the given printing policy.
      */
     """
 def clang_Range_isNull(arg0: CXSourceRange) -> int:
     """
     /**
-     * Returns non-zero if \p range is null.
+     * Returns non-zero if \\p range is null.
      */
     """
 def clang_TParamCommandComment_getDepth(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_TParamCommand AST node.
+     * \\param Comment a \\c CXComment_TParamCommand AST node.
      *
-     * \returns zero-based nesting depth of this parameter in the template parameter list.
+     * \\returns zero-based nesting depth of this parameter in the template parameter list.
      *
      * For example,
-     * \verbatim
+     * \\verbatim
      *     template<typename C, template<typename T> class TT>
      *     void test(TT<int> aaa);
-     * \endverbatim
+     * \\endverbatim
      * for C and TT nesting depth is 0,
      * for T nesting depth is 1.
      */
     """
 def clang_TParamCommandComment_getIndex(arg0: CXComment, arg1: int) -> int:
     """
     /**
-     * \param Comment a \c CXComment_TParamCommand AST node.
+     * \\param Comment a \\c CXComment_TParamCommand AST node.
      *
-     * \returns zero-based parameter index in the template parameter list at a
+     * \\returns zero-based parameter index in the template parameter list at a
      * given nesting depth.
      *
      * For example,
-     * \verbatim
+     * \\verbatim
      *     template<typename C, template<typename T> class TT>
      *     void test(TT<int> aaa);
-     * \endverbatim
+     * \\endverbatim
      * for C and TT nesting depth is 0, so we can ask for index at depth 0:
      * at depth 0 C's index is 0, TT's index is 1.
      *
      * For T nesting depth is 1, so we can ask for index at depth 0 and 1:
      * at depth 0 T's index is 1 (same as TT's),
      * at depth 1 T's index is 0.
      */
     """
 def clang_TParamCommandComment_getParamName(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_TParamCommand AST node.
+     * \\param Comment a \\c CXComment_TParamCommand AST node.
      *
-     * \returns template parameter name.
+     * \\returns template parameter name.
      */
     """
 def clang_TParamCommandComment_isParamPositionValid(arg0: CXComment) -> int:
     """
     /**
-     * \param Comment a \c CXComment_TParamCommand AST node.
+     * \\param Comment a \\c CXComment_TParamCommand AST node.
      *
-     * \returns non-zero if the parameter that this AST node represents was found
+     * \\returns non-zero if the parameter that this AST node represents was found
      * in the template parameter list and
-     * \c clang_TParamCommandComment_getDepth and
-     * \c clang_TParamCommandComment_getIndex functions will return a meaningful
+     * \\c clang_TParamCommandComment_getDepth and
+     * \\c clang_TParamCommandComment_getIndex functions will return a meaningful
      * value.
      */
     """
 def clang_TargetInfo_dispose(arg0: CXTargetInfoImplp) -> None:
     """
     /**
      * Destroy the CXTargetInfo object.
@@ -8252,17 +8758,17 @@
      *
      * Returns the empty string in case of any error.
      */
     """
 def clang_TextComment_getText(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_Text AST node.
+     * \\param Comment a \\c CXComment_Text AST node.
      *
-     * \returns text contained in the AST node.
+     * \\returns text contained in the AST node.
      */
     """
 def clang_Type_getAlignOf(arg0: CXType) -> int:
     """
     /**
      * Return the alignment of a type in bytes as per C++[expr.alignof]
      *   standard.
@@ -8331,15 +8837,15 @@
      * If the type is not an ObjC object, 0 is returned.
      */
     """
 def clang_Type_getNumTemplateArguments(arg0: CXType) -> int:
     """
     /**
      * Returns the number of template arguments for given template
-     * specialization, or -1 if type \c T is not a template specialization.
+     * specialization, or -1 if type \\c T is not a template specialization.
      */
     """
 def clang_Type_getObjCEncoding(arg0: CXType) -> CXString:
     """
     /**
      * Returns the Objective-C type encoding for the specified CXType.
      */
@@ -8420,129 +8926,129 @@
     """
     /**
      * Determine if a typedef is 'transparent' tag.
      *
      * A typedef is considered 'transparent' if it shares a name and spelling
      * location with its underlying tag type, as is the case with the NS_ENUM macro.
      *
-     * \returns non-zero if transparent and zero otherwise.
+     * \\returns non-zero if transparent and zero otherwise.
      */
     """
-def clang_Type_visitFields(arg0: CXType, arg1: typing.Callable[[pylibclang._C.CXCursor, pylibclang._C.voidp], CXVisitorResult], arg2: voidp) -> int:
+def clang_Type_visitFields(arg0: CXType, arg1: typing.Callable[[CXCursor, voidp], CXVisitorResult], arg2: voidp) -> int:
     """
     /**
      * Visit the fields of a particular type.
      *
      * This function visits all the direct fields of the given cursor,
-     * invoking the given \p visitor function with the cursors of each
+     * invoking the given \\p visitor function with the cursors of each
      * visited field. The traversal may be ended prematurely, if
-     * the visitor returns \c CXFieldVisit_Break.
+     * the visitor returns \\c CXFieldVisit_Break.
      *
-     * \param T the record type whose field may be visited.
+     * \\param T the record type whose field may be visited.
      *
-     * \param visitor the visitor function that will be invoked for each
-     * field of \p T.
+     * \\param visitor the visitor function that will be invoked for each
+     * field of \\p T.
      *
-     * \param client_data pointer data supplied by the client, which will
+     * \\param client_data pointer data supplied by the client, which will
      * be passed to the visitor each time it is invoked.
      *
-     * \returns a non-zero value if the traversal was terminated
-     * prematurely by the visitor returning \c CXFieldVisit_Break.
+     * \\returns a non-zero value if the traversal was terminated
+     * prematurely by the visitor returning \\c CXFieldVisit_Break.
      */
     """
 def clang_VerbatimBlockLineComment_getText(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_VerbatimBlockLine AST node.
+     * \\param Comment a \\c CXComment_VerbatimBlockLine AST node.
      *
-     * \returns text contained in the AST node.
+     * \\returns text contained in the AST node.
      */
     """
 def clang_VerbatimLineComment_getText(arg0: CXComment) -> CXString:
     """
     /**
-     * \param Comment a \c CXComment_VerbatimLine AST node.
+     * \\param Comment a \\c CXComment_VerbatimLine AST node.
      *
-     * \returns text contained in the AST node.
+     * \\returns text contained in the AST node.
      */
     """
 def clang_VirtualFileOverlay_addFileMapping(arg0: CXVirtualFileOverlayImplp, arg1: str, arg2: str) -> CXErrorCode:
     """
     /**
      * Map an absolute virtual file path to an absolute real one.
      * The virtual path must be canonicalized (not contain "."/"..").
-     * \returns 0 for success, non-zero to indicate an error.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_VirtualFileOverlay_create(arg0: int) -> CXVirtualFileOverlayImplp:
     """
     /**
-     * Create a \c CXVirtualFileOverlay object.
-     * Must be disposed with \c clang_VirtualFileOverlay_dispose().
+     * Create a \\c CXVirtualFileOverlay object.
+     * Must be disposed with \\c clang_VirtualFileOverlay_dispose().
      *
-     * \param options is reserved, always pass 0.
+     * \\param options is reserved, always pass 0.
      */
     """
 def clang_VirtualFileOverlay_dispose(arg0: CXVirtualFileOverlayImplp) -> None:
     """
     /**
-     * Dispose a \c CXVirtualFileOverlay object.
+     * Dispose a \\c CXVirtualFileOverlay object.
      */
     """
 def clang_VirtualFileOverlay_setCaseSensitivity(arg0: CXVirtualFileOverlayImplp, arg1: int) -> CXErrorCode:
     """
     /**
-     * Set the case sensitivity for the \c CXVirtualFileOverlay object.
-     * The \c CXVirtualFileOverlay object is case-sensitive by default, this
+     * Set the case sensitivity for the \\c CXVirtualFileOverlay object.
+     * The \\c CXVirtualFileOverlay object is case-sensitive by default, this
      * option can be used to override the default.
-     * \returns 0 for success, non-zero to indicate an error.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_VirtualFileOverlay_writeToBuffer(arg0: CXVirtualFileOverlayImplp, arg1: int, arg2: charpp, arg3: int) -> CXErrorCode:
     """
     /**
-     * Write out the \c CXVirtualFileOverlay object to a char buffer.
+     * Write out the \\c CXVirtualFileOverlay object to a char buffer.
      *
-     * \param options is reserved, always pass 0.
-     * \param out_buffer_ptr pointer to receive the buffer pointer, which should be
-     * disposed using \c clang_free().
-     * \param out_buffer_size pointer to receive the buffer size.
-     * \returns 0 for success, non-zero to indicate an error.
+     * \\param options is reserved, always pass 0.
+     * \\param out_buffer_ptr pointer to receive the buffer pointer, which should be
+     * disposed using \\c clang_free().
+     * \\param out_buffer_size pointer to receive the buffer size.
+     * \\returns 0 for success, non-zero to indicate an error.
      */
     """
 def clang_annotateTokens(arg0: CXTranslationUnitImplp, arg1: CXToken, arg2: int, arg3: CXCursor) -> None:
     """
     /**
      * Annotate the given set of tokens by providing cursors for each token
      * that can be mapped to a specific entity within the abstract syntax tree.
      *
      * This token-annotation routine is equivalent to invoking
      * clang_getCursor() for the source locations of each of the
      * tokens. The cursors provided are filtered, so that only those
      * cursors that have a direct correspondence to the token are
-     * accepted. For example, given a function call \c f(x),
+     * accepted. For example, given a function call \\c f(x),
      * clang_getCursor() would provide the following cursors:
      *
      *   * when the cursor is over the 'f', a DeclRefExpr cursor referring to 'f'.
      *   * when the cursor is over the '(' or the ')', a CallExpr referring to 'f'.
      *   * when the cursor is over the 'x', a DeclRefExpr cursor referring to 'x'.
      *
      * Only the first and last of these cursors will occur within the
      * annotate, since the tokens "f" and "x' directly refer to a function
      * and a variable, respectively, but the parentheses are just a small
      * part of the full syntax of the function call expression, which is
      * not provided as an annotation.
      *
-     * \param TU the translation unit that owns the given tokens.
+     * \\param TU the translation unit that owns the given tokens.
      *
-     * \param Tokens the set of tokens to annotate.
+     * \\param Tokens the set of tokens to annotate.
      *
-     * \param NumTokens the number of tokens in \p Tokens.
+     * \\param NumTokens the number of tokens in \\p Tokens.
      *
-     * \param Cursors an array of \p NumTokens cursors, whose contents will be
+     * \\param Cursors an array of \\p NumTokens cursors, whose contents will be
      * replaced with the cursors corresponding to each token.
      */
     """
 def clang_codeCompleteAt(arg0: CXTranslationUnitImplp, arg1: str, arg2: int, arg3: int, arg4: CXUnsavedFile, arg5: int, arg6: int) -> CXCodeCompleteResults:
     """
     /**
      * Perform code completion at a given location in a translation unit.
@@ -8552,124 +9058,124 @@
      * code snippets based on the context of the completion. The basic model
      * for code completion is that Clang will parse a complete source file,
      * performing syntax checking up to the location where code-completion has
      * been requested. At that point, a special code-completion token is passed
      * to the parser, which recognizes this token and determines, based on the
      * current location in the C/Objective-C/C++ grammar and the state of
      * semantic analysis, what completions to provide. These completions are
-     * returned via a new \c CXCodeCompleteResults structure.
+     * returned via a new \\c CXCodeCompleteResults structure.
      *
      * Code completion itself is meant to be triggered by the client when the
      * user types punctuation characters or whitespace, at which point the
-     * code-completion location will coincide with the cursor. For example, if \c p
+     * code-completion location will coincide with the cursor. For example, if \\c p
      * is a pointer, code-completion might be triggered after the "-" and then
-     * after the ">" in \c p->. When the code-completion location is after the ">",
+     * after the ">" in \\c p->. When the code-completion location is after the ">",
      * the completion results will provide, e.g., the members of the struct that
      * "p" points to. The client is responsible for placing the cursor at the
      * beginning of the token currently being typed, then filtering the results
      * based on the contents of the token. For example, when code-completing for
-     * the expression \c p->get, the client should provide the location just after
+     * the expression \\c p->get, the client should provide the location just after
      * the ">" (e.g., pointing at the "g") to this code-completion hook. Then, the
      * client can filter the results based on the current token text ("get"), only
      * showing those results that start with "get". The intent of this interface
      * is to separate the relatively high-latency acquisition of code-completion
      * results from the filtering of results on a per-character basis, which must
      * have a lower latency.
      *
-     * \param TU The translation unit in which code-completion should
+     * \\param TU The translation unit in which code-completion should
      * occur. The source files for this translation unit need not be
      * completely up-to-date (and the contents of those source files may
-     * be overridden via \p unsaved_files). Cursors referring into the
+     * be overridden via \\p unsaved_files). Cursors referring into the
      * translation unit may be invalidated by this invocation.
      *
-     * \param complete_filename The name of the source file where code
+     * \\param complete_filename The name of the source file where code
      * completion should be performed. This filename may be any file
      * included in the translation unit.
      *
-     * \param complete_line The line at which code-completion should occur.
+     * \\param complete_line The line at which code-completion should occur.
      *
-     * \param complete_column The column at which code-completion should occur.
+     * \\param complete_column The column at which code-completion should occur.
      * Note that the column should point just after the syntactic construct that
      * initiated code completion, and not in the middle of a lexical token.
      *
-     * \param unsaved_files the Files that have not yet been saved to disk
+     * \\param unsaved_files the Files that have not yet been saved to disk
      * but may be required for parsing or code completion, including the
      * contents of those files.  The contents and name of these files (as
      * specified by CXUnsavedFile) are copied when necessary, so the
      * client only needs to guarantee their validity until the call to
      * this function returns.
      *
-     * \param num_unsaved_files The number of unsaved file entries in \p
+     * \\param num_unsaved_files The number of unsaved file entries in \\p
      * unsaved_files.
      *
-     * \param options Extra options that control the behavior of code
+     * \\param options Extra options that control the behavior of code
      * completion, expressed as a bitwise OR of the enumerators of the
      * CXCodeComplete_Flags enumeration. The
-     * \c clang_defaultCodeCompleteOptions() function returns a default set
+     * \\c clang_defaultCodeCompleteOptions() function returns a default set
      * of code-completion options.
      *
-     * \returns If successful, a new \c CXCodeCompleteResults structure
+     * \\returns If successful, a new \\c CXCodeCompleteResults structure
      * containing code-completion results, which should eventually be
-     * freed with \c clang_disposeCodeCompleteResults(). If code
+     * freed with \\c clang_disposeCodeCompleteResults(). If code
      * completion fails, returns NULL.
      */
     """
 def clang_codeCompleteGetContainerKind(arg0: CXCodeCompleteResults, arg1: int) -> CXCursorKind:
     """
     /**
      * Returns the cursor kind for the container for the current code
      * completion context. The container is only guaranteed to be set for
      * contexts where a container exists (i.e. member accesses or Objective-C
      * message sends); if there is not a container, this function will return
      * CXCursor_InvalidCode.
      *
-     * \param Results the code completion results to query
+     * \\param Results the code completion results to query
      *
-     * \param IsIncomplete on return, this value will be false if Clang has complete
+     * \\param IsIncomplete on return, this value will be false if Clang has complete
      * information about the container. If Clang does not have complete
      * information, this value will be true.
      *
-     * \returns the container kind, or CXCursor_InvalidCode if there is not a
+     * \\returns the container kind, or CXCursor_InvalidCode if there is not a
      * container
      */
     """
 def clang_codeCompleteGetContainerUSR(arg0: CXCodeCompleteResults) -> CXString:
     """
     /**
      * Returns the USR for the container for the current code completion
      * context. If there is not a container for the current context, this
      * function will return the empty string.
      *
-     * \param Results the code completion results to query
+     * \\param Results the code completion results to query
      *
-     * \returns the USR for the container
+     * \\returns the USR for the container
      */
     """
 def clang_codeCompleteGetContexts(arg0: CXCodeCompleteResults) -> int:
     """
     /**
      * Determines what completions are appropriate for the context
      * the given code completion.
      *
-     * \param Results the code completion results to query
+     * \\param Results the code completion results to query
      *
-     * \returns the kinds of completions that are appropriate for use
+     * \\returns the kinds of completions that are appropriate for use
      * along with the given code completion results.
      */
     """
 def clang_codeCompleteGetDiagnostic(arg0: CXCodeCompleteResults, arg1: int) -> voidp:
     """
     /**
      * Retrieve a diagnostic associated with the given code completion.
      *
-     * \param Results the code completion results to query.
-     * \param Index the zero-based diagnostic number to retrieve.
+     * \\param Results the code completion results to query.
+     * \\param Index the zero-based diagnostic number to retrieve.
      *
-     * \returns the requested diagnostic. This diagnostic must be freed
-     * via a call to \c clang_disposeDiagnostic().
+     * \\returns the requested diagnostic. This diagnostic must be freed
+     * via a call to \\c clang_disposeDiagnostic().
      */
     """
 def clang_codeCompleteGetNumDiagnostics(arg0: CXCodeCompleteResults) -> int:
     """
     /**
      * Determine the number of diagnostics produced prior to the
      * location where code completion was performed.
@@ -8679,17 +9185,17 @@
     """
     /**
      * Returns the currently-entered selector for an Objective-C message
      * send, formatted like "initWithFoo:bar:". Only guaranteed to return a
      * non-empty string for CXCompletionContext_ObjCInstanceMessage and
      * CXCompletionContext_ObjCClassMessage.
      *
-     * \param Results the code completion results to query
+     * \\param Results the code completion results to query
      *
-     * \returns the selector (or partial selector) that has been entered thus far
+     * \\returns the selector (or partial selector) that has been entered thus far
      * for an Objective-C message send.
      */
     """
 def clang_constructUSR_ObjCCategory(arg0: str, arg1: str) -> CXString:
     """
     /**
      * Construct a USR for a specified Objective-C category.
@@ -8727,22 +9233,22 @@
     /**
      * Construct a USR for a specified Objective-C protocol.
      */
     """
 def clang_createAPISet(arg0: CXTranslationUnitImplp, arg1: CXAPISetImplpp) -> CXErrorCode:
     """
     /**
-     * Traverses the translation unit to create a \c CXAPISet.
+     * Traverses the translation unit to create a \\c CXAPISet.
      *
-     * \param tu is the \c CXTranslationUnit to build the \c CXAPISet for.
+     * \\param tu is the \\c CXTranslationUnit to build the \\c CXAPISet for.
      *
-     * \param out_api is a pointer to the output of this function. It is needs to be
+     * \\param out_api is a pointer to the output of this function. It is needs to be
      * disposed of by calling clang_disposeAPISet.
      *
-     * \returns Error code indicating success or failure of the APISet creation.
+     * \\returns Error code indicating success or failure of the APISet creation.
      */
     """
 def clang_createCXCursorSet() -> CXCursorSetImplp:
     """
     /**
      * Creates an empty CXCursorSet.
      */
@@ -8758,15 +9264,15 @@
      * declarations (when loading any new translation units). A "local" declaration
      * is one that belongs in the translation unit itself and not in a precompiled
      * header that was used by the translation unit. If zero, all declarations
      * will be enumerated.
      *
      * Here is an example:
      *
-     * \code
+     * \\code
      *   // excludeDeclsFromPCH = 1, displayDiagnostics=1
      *   Idx = clang_createIndex(1, 1);
      *
      *   // IndexTest.pch was produced with the following command:
      *   // "clang -x c IndexTest.h -emit-ast -o IndexTest.pch"
      *   TU = clang_createTranslationUnit(Idx, "IndexTest.pch");
      *
@@ -8779,39 +9285,85 @@
      *   // from 'IndexTest.pch'.
      *   char *args[] = { "-Xclang", "-include-pch=IndexTest.pch" };
      *   TU = clang_createTranslationUnitFromSourceFile(Idx, "IndexTest.c", 2, args,
      *                                                  0, 0);
      *   clang_visitChildren(clang_getTranslationUnitCursor(TU),
      *                       TranslationUnitVisitor, 0);
      *   clang_disposeTranslationUnit(TU);
-     * \endcode
+     * \\endcode
      *
      * This process of creating the 'pch', loading it separately, and using it (via
      * -include-pch) allows 'excludeDeclsFromPCH' to remove redundant callbacks
      * (which gives the indexer the same performance benefit as the compiler).
      */
     """
+def clang_createIndexWithOptions(arg0: CXIndexOptions) -> voidp:
+    """
+    /**
+     * Provides a shared context for creating translation units.
+     *
+     * Call this function instead of clang_createIndex() if you need to configure
+     * the additional options in CXIndexOptions.
+     *
+     * \\returns The created index or null in case of error, such as an unsupported
+     * value of options->Size.
+     *
+     * For example:
+     * \\code
+     * CXIndex createIndex(const char *ApplicationTemporaryPath) {
+     *   const int ExcludeDeclarationsFromPCH = 1;
+     *   const int DisplayDiagnostics = 1;
+     *   CXIndex Idx;
+     * #if CINDEX_VERSION_MINOR >= 64
+     *   CXIndexOptions Opts;
+     *   memset(&Opts, 0, sizeof(Opts));
+     *   Opts.Size = sizeof(CXIndexOptions);
+     *   Opts.ThreadBackgroundPriorityForIndexing = 1;
+     *   Opts.ExcludeDeclarationsFromPCH = ExcludeDeclarationsFromPCH;
+     *   Opts.DisplayDiagnostics = DisplayDiagnostics;
+     *   Opts.PreambleStoragePath = ApplicationTemporaryPath;
+     *   Idx = clang_createIndexWithOptions(&Opts);
+     *   if (Idx)
+     *     return Idx;
+     *   fprintf(stderr,
+     *           "clang_createIndexWithOptions() failed. "
+     *           "CINDEX_VERSION_MINOR = %d, sizeof(CXIndexOptions) = %u\\n",
+     *           CINDEX_VERSION_MINOR, Opts.Size);
+     * #else
+     *   (void)ApplicationTemporaryPath;
+     * #endif
+     *   Idx = clang_createIndex(ExcludeDeclarationsFromPCH, DisplayDiagnostics);
+     *   clang_CXIndex_setGlobalOptions(
+     *       Idx, clang_CXIndex_getGlobalOptions(Idx) |
+     *                CXGlobalOpt_ThreadBackgroundPriorityForIndexing);
+     *   return Idx;
+     * }
+     * \\endcode
+     *
+     * \\sa clang_createIndex()
+     */
+    """
 def clang_createTranslationUnit(arg0: voidp, arg1: str) -> CXTranslationUnitImplp:
     """
     /**
-     * Same as \c clang_createTranslationUnit2, but returns
-     * the \c CXTranslationUnit instead of an error code.  In case of an error this
-     * routine returns a \c NULL \c CXTranslationUnit, without further detailed
+     * Same as \\c clang_createTranslationUnit2, but returns
+     * the \\c CXTranslationUnit instead of an error code.  In case of an error this
+     * routine returns a \\c NULL \\c CXTranslationUnit, without further detailed
      * error codes.
      */
     """
 def clang_createTranslationUnit2(arg0: voidp, arg1: str, arg2: CXTranslationUnitImplpp) -> CXErrorCode:
     """
     /**
-     * Create a translation unit from an AST file (\c -emit-ast).
+     * Create a translation unit from an AST file (\\c -emit-ast).
      *
-     * \param[out] out_TU A non-NULL pointer to store the created
-     * \c CXTranslationUnit.
+     * \\param[out] out_TU A non-NULL pointer to store the created
+     * \\c CXTranslationUnit.
      *
-     * \returns Zero on success, otherwise returns an error code.
+     * \\returns Zero on success, otherwise returns an error code.
      */
     """
 def clang_createTranslationUnitFromSourceFile(arg0: voidp, arg1: str, arg2: int, arg3: constcharpconstp, arg4: int, arg5: CXUnsavedFile) -> CXTranslationUnitImplp:
     """
     /**
      * Return the CXTranslationUnit for a given source file and the provided
      * command line arguments one would pass to the compiler.
@@ -8822,116 +9374,116 @@
      *
      * Note: When encountered in 'clang_command_line_args', the following options
      * are ignored:
      *
      *   '-c'
      *   '-emit-ast'
      *   '-fsyntax-only'
-     *   '-o \<output file>'  (both '-o' and '\<output file>' are ignored)
+     *   '-o \\<output file>'  (both '-o' and '\\<output file>' are ignored)
      *
-     * \param CIdx The index object with which the translation unit will be
+     * \\param CIdx The index object with which the translation unit will be
      * associated.
      *
-     * \param source_filename The name of the source file to load, or NULL if the
-     * source file is included in \p clang_command_line_args.
+     * \\param source_filename The name of the source file to load, or NULL if the
+     * source file is included in \\p clang_command_line_args.
      *
-     * \param num_clang_command_line_args The number of command-line arguments in
-     * \p clang_command_line_args.
+     * \\param num_clang_command_line_args The number of command-line arguments in
+     * \\p clang_command_line_args.
      *
-     * \param clang_command_line_args The command-line arguments that would be
-     * passed to the \c clang executable if it were being invoked out-of-process.
+     * \\param clang_command_line_args The command-line arguments that would be
+     * passed to the \\c clang executable if it were being invoked out-of-process.
      * These command-line options will be parsed and will affect how the translation
      * unit is parsed. Note that the following options are ignored: '-c',
-     * '-emit-ast', '-fsyntax-only' (which is the default), and '-o \<output file>'.
+     * '-emit-ast', '-fsyntax-only' (which is the default), and '-o \\<output file>'.
      *
-     * \param num_unsaved_files the number of unsaved file entries in \p
+     * \\param num_unsaved_files the number of unsaved file entries in \\p
      * unsaved_files.
      *
-     * \param unsaved_files the files that have not yet been saved to disk
+     * \\param unsaved_files the files that have not yet been saved to disk
      * but may be required for code completion, including the contents of
      * those files.  The contents and name of these files (as specified by
      * CXUnsavedFile) are copied when necessary, so the client only needs to
      * guarantee their validity until the call to this function returns.
      */
     """
 def clang_defaultCodeCompleteOptions() -> int:
     """
     /**
      * Returns a default set of code-completion options that can be
-     * passed to\c clang_codeCompleteAt().
+     * passed to\\c clang_codeCompleteAt().
      */
     """
 def clang_defaultDiagnosticDisplayOptions() -> int:
     """
     /**
      * Retrieve the set of display options most similar to the
      * default behavior of the clang compiler.
      *
-     * \returns A set of display options suitable for use with \c
+     * \\returns A set of display options suitable for use with \\c
      * clang_formatDiagnostic().
      */
     """
 def clang_defaultEditingTranslationUnitOptions() -> int:
     """
     /**
      * Returns the set of flags that is suitable for parsing a translation
      * unit that is being edited.
      *
-     * The set of flags returned provide options for \c clang_parseTranslationUnit()
+     * The set of flags returned provide options for \\c clang_parseTranslationUnit()
      * to indicate that the translation unit is likely to be reparsed many times,
-     * either explicitly (via \c clang_reparseTranslationUnit()) or implicitly
-     * (e.g., by code completion (\c clang_codeCompletionAt())). The returned flag
+     * either explicitly (via \\c clang_reparseTranslationUnit()) or implicitly
+     * (e.g., by code completion (\\c clang_codeCompletionAt())). The returned flag
      * set contains an unspecified set of optimizations (e.g., the precompiled
      * preamble) geared toward improving the performance of these routines. The
      * set of optimizations enabled may change from one version to the next.
      */
     """
 def clang_defaultReparseOptions(arg0: CXTranslationUnitImplp) -> int:
     """
     /**
      * Returns the set of flags that is suitable for reparsing a translation
      * unit.
      *
      * The set of flags returned provide options for
-     * \c clang_reparseTranslationUnit() by default. The returned flag
+     * \\c clang_reparseTranslationUnit() by default. The returned flag
      * set contains an unspecified set of optimizations geared toward common uses
      * of reparsing. The set of optimizations enabled may change from one version
      * to the next.
      */
     """
 def clang_defaultSaveOptions(arg0: CXTranslationUnitImplp) -> int:
     """
     /**
      * Returns the set of flags that is suitable for saving a translation
      * unit.
      *
      * The set of flags returned provide options for
-     * \c clang_saveTranslationUnit() by default. The returned flag
+     * \\c clang_saveTranslationUnit() by default. The returned flag
      * set contains an unspecified set of options that save translation units with
      * the most commonly-requested data.
      */
     """
 def clang_disposeAPISet(arg0: CXAPISetImplp) -> None:
     """
     /**
      * Dispose of an APISet.
      *
-     * The provided \c CXAPISet can not be used after this function is called.
+     * The provided \\c CXAPISet can not be used after this function is called.
      */
     """
 def clang_disposeCXCursorSet(arg0: CXCursorSetImplp) -> None:
     """
     /**
      * Disposes a CXCursorSet and releases its associated memory.
      */
     """
 def clang_disposeCXPlatformAvailability(arg0: CXPlatformAvailability) -> None:
     """
     /**
-     * Free the memory associated with a \c CXPlatformAvailability structure.
+     * Free the memory associated with a \\c CXPlatformAvailability structure.
      */
     """
 def clang_disposeCXTUResourceUsage(arg0: CXTUResourceUsage) -> None:
     ...
 def clang_disposeCodeCompleteResults(arg0: CXCodeCompleteResults) -> None:
     """
     /**
@@ -8958,22 +9510,22 @@
      * The index must not be destroyed until all of the translation units created
      * within that index have been destroyed.
      */
     """
 def clang_disposeOverriddenCursors(arg0: CXCursor) -> None:
     """
     /**
-     * Free the set of overridden cursors returned by \c
+     * Free the set of overridden cursors returned by \\c
      * clang_getOverriddenCursors().
      */
     """
 def clang_disposeSourceRangeList(arg0: CXSourceRangeList) -> None:
     """
     /**
-     * Destroy the given \c CXSourceRangeList.
+     * Destroy the given \\c CXSourceRangeList.
      */
     """
 def clang_disposeString(arg0: CXString) -> None:
     """
     /**
      * Free the given string.
      */
@@ -9007,94 +9559,98 @@
 def clang_equalLocations(arg0: CXSourceLocation, arg1: CXSourceLocation) -> int:
     """
     /**
      * Determine whether two source locations, which must refer into
      * the same translation unit, refer to exactly the same point in the source
      * code.
      *
-     * \returns non-zero if the source locations refer to the same location, zero
+     * \\returns non-zero if the source locations refer to the same location, zero
      * if they refer to different locations.
      */
     """
 def clang_equalRanges(arg0: CXSourceRange, arg1: CXSourceRange) -> int:
     """
     /**
      * Determine whether two ranges are equivalent.
      *
-     * \returns non-zero if the ranges are the same, zero if they differ.
+     * \\returns non-zero if the ranges are the same, zero if they differ.
      */
     """
 def clang_equalTypes(arg0: CXType, arg1: CXType) -> int:
     """
     /**
      * Determine whether two CXTypes represent the same type.
      *
-     * \returns non-zero if the CXTypes represent the same type and
+     * \\returns non-zero if the CXTypes represent the same type and
      *          zero otherwise.
      */
     """
-def clang_executeOnThread(arg0: typing.Callable[[pylibclang._C.voidp], None], arg1: voidp, arg2: int) -> None:
+def clang_executeOnThread(arg0: typing.Callable[[voidp], None], arg1: voidp, arg2: int) -> None:
     ...
 def clang_findIncludesInFile(arg0: CXTranslationUnitImplp, arg1: voidp, arg2: CXCursorAndRangeVisitor) -> CXResult:
     """
     /**
      * Find #import/#include directives in a specific file.
      *
-     * \param TU translation unit containing the file to query.
+     * \\param TU translation unit containing the file to query.
      *
-     * \param file to search for #import/#include directives.
+     * \\param file to search for #import/#include directives.
      *
-     * \param visitor callback that will receive pairs of CXCursor/CXSourceRange for
+     * \\param visitor callback that will receive pairs of CXCursor/CXSourceRange for
      * each directive found.
      *
-     * \returns one of the CXResult enumerators.
+     * \\returns one of the CXResult enumerators.
      */
     """
+def clang_findIncludesInFileWithBlock(arg0: CXTranslationUnitImplp, arg1: voidp, arg2: _CXCursorAndRangeVisitorBlockp) -> CXResult:
+    ...
 def clang_findReferencesInFile(arg0: CXCursor, arg1: voidp, arg2: CXCursorAndRangeVisitor) -> CXResult:
     """
     /**
      * Find references of a declaration in a specific file.
      *
-     * \param cursor pointing to a declaration or a reference of one.
+     * \\param cursor pointing to a declaration or a reference of one.
      *
-     * \param file to search for references.
+     * \\param file to search for references.
      *
-     * \param visitor callback that will receive pairs of CXCursor/CXSourceRange for
+     * \\param visitor callback that will receive pairs of CXCursor/CXSourceRange for
      * each reference found.
      * The CXSourceRange will point inside the file; if the reference is inside
      * a macro (and not a macro argument) the CXSourceRange will be invalid.
      *
-     * \returns one of the CXResult enumerators.
+     * \\returns one of the CXResult enumerators.
      */
     """
+def clang_findReferencesInFileWithBlock(arg0: CXCursor, arg1: voidp, arg2: _CXCursorAndRangeVisitorBlockp) -> CXResult:
+    ...
 def clang_formatDiagnostic(arg0: voidp, arg1: int) -> CXString:
     """
     /**
      * Format the given diagnostic in a manner that is suitable for display.
      *
      * This routine will format the given diagnostic to a string, rendering
      * the diagnostic according to the various options given. The
-     * \c clang_defaultDiagnosticDisplayOptions() function returns the set of
+     * \\c clang_defaultDiagnosticDisplayOptions() function returns the set of
      * options that most closely mimics the behavior of the clang compiler.
      *
-     * \param Diagnostic The diagnostic to print.
+     * \\param Diagnostic The diagnostic to print.
      *
-     * \param Options A set of options that control the diagnostic display,
-     * created by combining \c CXDiagnosticDisplayOptions values.
+     * \\param Options A set of options that control the diagnostic display,
+     * created by combining \\c CXDiagnosticDisplayOptions values.
      *
-     * \returns A new string containing for formatted diagnostic.
+     * \\returns A new string containing for formatted diagnostic.
      */
     """
 def clang_free(arg0: voidp) -> None:
     """
     /**
      * free memory allocated by libclang, such as the buffer returned by
-     * \c CXVirtualFileOverlay() or \c clang_ModuleMapDescriptor_writeToBuffer().
+     * \\c CXVirtualFileOverlay() or \\c clang_ModuleMapDescriptor_writeToBuffer().
      *
-     * \param buffer memory pointer to free.
+     * \\param buffer memory pointer to free.
      */
     """
 def clang_getAddressSpace(arg0: CXType) -> int:
     """
     /**
      * Returns the address space of the given type.
      */
@@ -9130,19 +9686,25 @@
     """
     /**
      * Return the array size of a constant array.
      *
      * If a non-array type is passed in, -1 is returned.
      */
     """
+def clang_getBinaryOperatorKindSpelling(arg0: CXBinaryOperatorKind) -> CXString:
+    """
+    /**
+     * Retrieve the spelling of a given CXBinaryOperatorKind.
+     */
+    """
 def clang_getBuildSessionTimestamp() -> int:
     """
     /**
      * Return the timestamp for use with Clang's
-     * \c -fbuild-session-timestamp= option.
+     * \\c -fbuild-session-timestamp= option.
      */
     """
 def clang_getCString(arg0: CXString) -> str:
     """
     /**
      * Retrieve the character data associated with the given string.
      */
@@ -9169,30 +9731,30 @@
     /**
      * Retrieve the canonical cursor corresponding to the given cursor.
      *
      * In the C family of languages, many kinds of entities can be declared several
      * times within a single translation unit. For example, a structure type can
      * be forward-declared (possibly multiple times) and later defined:
      *
-     * \code
+     * \\code
      * struct X;
      * struct X;
      * struct X {
      *   int member;
      * };
-     * \endcode
+     * \\endcode
      *
-     * The declarations and the definition of \c X are represented by three
+     * The declarations and the definition of \\c X are represented by three
      * different cursors, all of which are declarations of the same underlying
      * entity. One of these cursor is considered the "canonical" cursor, which
      * is effectively the representative for the underlying entity. One can
      * determine if two cursors are declarations of the same underlying entity by
      * comparing their canonical cursors.
      *
-     * \returns The canonical cursor for the entity referred to by the given cursor.
+     * \\returns The canonical cursor for the entity referred to by the given cursor.
      */
     """
 def clang_getCanonicalType(arg0: CXType) -> CXType:
     """
     /**
      * Return the canonical type for a CXType.
      *
@@ -9219,32 +9781,32 @@
      */
     """
 def clang_getCompletionAnnotation(arg0: voidp, arg1: int) -> CXString:
     """
     /**
      * Retrieve the annotation associated with the given completion string.
      *
-     * \param completion_string the completion string to query.
+     * \\param completion_string the completion string to query.
      *
-     * \param annotation_number the 0-based index of the annotation of the
+     * \\param annotation_number the 0-based index of the annotation of the
      * completion string.
      *
-     * \returns annotation string associated with the completion at index
-     * \c annotation_number, or a NULL string if that annotation is not available.
+     * \\returns annotation string associated with the completion at index
+     * \\c annotation_number, or a NULL string if that annotation is not available.
      */
     """
 def clang_getCompletionAvailability(arg0: voidp) -> CXAvailabilityKind:
     """
     /**
      * Determine the availability of the entity that this code-completion
      * string refers to.
      *
-     * \param completion_string The completion string to query.
+     * \\param completion_string The completion string to query.
      *
-     * \returns The availability of the completion string.
+     * \\returns The availability of the completion string.
      */
     """
 def clang_getCompletionBriefComment(arg0: voidp) -> CXString:
     """
     /**
      * Retrieve the brief documentation comment attached to the declaration
      * that corresponds to the given completion string.
@@ -9252,45 +9814,45 @@
     """
 def clang_getCompletionChunkCompletionString(arg0: voidp, arg1: int) -> voidp:
     """
     /**
      * Retrieve the completion string associated with a particular chunk
      * within a completion string.
      *
-     * \param completion_string the completion string to query.
+     * \\param completion_string the completion string to query.
      *
-     * \param chunk_number the 0-based index of the chunk in the completion string.
+     * \\param chunk_number the 0-based index of the chunk in the completion string.
      *
-     * \returns the completion string associated with the chunk at index
-     * \c chunk_number.
+     * \\returns the completion string associated with the chunk at index
+     * \\c chunk_number.
      */
     """
 def clang_getCompletionChunkKind(arg0: voidp, arg1: int) -> CXCompletionChunkKind:
     """
     /**
      * Determine the kind of a particular chunk within a completion string.
      *
-     * \param completion_string the completion string to query.
+     * \\param completion_string the completion string to query.
      *
-     * \param chunk_number the 0-based index of the chunk in the completion string.
+     * \\param chunk_number the 0-based index of the chunk in the completion string.
      *
-     * \returns the kind of the chunk at the index \c chunk_number.
+     * \\returns the kind of the chunk at the index \\c chunk_number.
      */
     """
 def clang_getCompletionChunkText(arg0: voidp, arg1: int) -> CXString:
     """
     /**
      * Retrieve the text associated with a particular chunk within a
      * completion string.
      *
-     * \param completion_string the completion string to query.
+     * \\param completion_string the completion string to query.
      *
-     * \param chunk_number the 0-based index of the chunk in the completion string.
+     * \\param chunk_number the 0-based index of the chunk in the completion string.
      *
-     * \returns the text associated with the chunk at index \c chunk_number.
+     * \\returns the text associated with the chunk at index \\c chunk_number.
      */
     """
 def clang_getCompletionFixIt(arg0: CXCodeCompleteResults, arg1: int, arg2: int, arg3: CXSourceRange) -> CXString:
     """
     /**
      * Fix-its that *must* be applied before inserting the text for the
      * corresponding completion.
@@ -9317,148 +9879,156 @@
      *
      * std::unique_ptr<std::vector<int>> vec_ptr;
      * In 'vec_ptr.^', one of the completions is 'push_back', it requires
      * replacing '.' with '->'.
      * In 'vec_ptr->^', one of the completions is 'release', it requires
      * replacing '->' with '.'.
      *
-     * \param results The structure keeping all completion results
+     * \\param results The structure keeping all completion results
      *
-     * \param completion_index The index of the completion
+     * \\param completion_index The index of the completion
      *
-     * \param fixit_index The index of the fix-it for the completion at
+     * \\param fixit_index The index of the fix-it for the completion at
      * completion_index
      *
-     * \param replacement_range The fix-it range that must be replaced before the
+     * \\param replacement_range The fix-it range that must be replaced before the
      * completion at completion_index can be applied
      *
-     * \returns The fix-it string that must replace the code at replacement_range
+     * \\returns The fix-it string that must replace the code at replacement_range
      * before the completion at completion_index can be applied
      */
     """
 def clang_getCompletionNumAnnotations(arg0: voidp) -> int:
     """
     /**
      * Retrieve the number of annotations associated with the given
      * completion string.
      *
-     * \param completion_string the completion string to query.
+     * \\param completion_string the completion string to query.
      *
-     * \returns the number of annotations associated with the given completion
+     * \\returns the number of annotations associated with the given completion
      * string.
      */
     """
 def clang_getCompletionNumFixIts(arg0: CXCodeCompleteResults, arg1: int) -> int:
     """
     /**
      * Retrieve the number of fix-its for the given completion index.
      *
      * Calling this makes sense only if CXCodeComplete_IncludeCompletionsWithFixIts
      * option was set.
      *
-     * \param results The structure keeping all completion results
+     * \\param results The structure keeping all completion results
      *
-     * \param completion_index The index of the completion
+     * \\param completion_index The index of the completion
      *
-     * \return The number of fix-its which must be applied before the completion at
+     * \\return The number of fix-its which must be applied before the completion at
      * completion_index can be applied
      */
     """
 def clang_getCompletionParent(arg0: voidp, arg1: CXCursorKind) -> CXString:
     """
     /**
      * Retrieve the parent context of the given completion string.
      *
      * The parent context of a completion string is the semantic parent of
      * the declaration (if any) that the code completion represents. For example,
      * a code completion for an Objective-C method would have the method's class
      * or protocol as its context.
      *
-     * \param completion_string The code completion string whose parent is
+     * \\param completion_string The code completion string whose parent is
      * being queried.
      *
-     * \param kind DEPRECATED: always set to CXCursor_NotImplemented if non-NULL.
+     * \\param kind DEPRECATED: always set to CXCursor_NotImplemented if non-NULL.
      *
-     * \returns The name of the completion parent, e.g., "NSObject" if
+     * \\returns The name of the completion parent, e.g., "NSObject" if
      * the completion string represents a method in the NSObject class.
      */
     """
 def clang_getCompletionPriority(arg0: voidp) -> int:
     """
     /**
      * Determine the priority of this code completion.
      *
      * The priority of a code completion indicates how likely it is that this
      * particular completion is the completion that the user will select. The
      * priority is selected by various internal heuristics.
      *
-     * \param completion_string The completion string to query.
+     * \\param completion_string The completion string to query.
      *
-     * \returns The priority of this completion string. Smaller values indicate
+     * \\returns The priority of this completion string. Smaller values indicate
      * higher-priority (more likely) completions.
      */
     """
 def clang_getCursor(arg0: CXTranslationUnitImplp, arg1: CXSourceLocation) -> CXCursor:
     """
     /**
      * Map a source location to the cursor that describes the entity at that
      * location in the source code.
      *
      * clang_getCursor() maps an arbitrary source location within a translation
      * unit down to the most specific cursor that describes the entity at that
-     * location. For example, given an expression \c x + y, invoking
+     * location. For example, given an expression \\c x + y, invoking
      * clang_getCursor() with a source location pointing to "x" will return the
      * cursor for "x"; similarly for "y". If the cursor points anywhere between
      * "x" or "y" (e.g., on the + or the whitespace around it), clang_getCursor()
      * will return a cursor referring to the "+" expression.
      *
-     * \returns a cursor representing the entity at the given source location, or
+     * \\returns a cursor representing the entity at the given source location, or
      * a NULL cursor if no such entity can be found.
      */
     """
 def clang_getCursorAvailability(arg0: CXCursor) -> CXAvailabilityKind:
     """
     /**
      * Determine the availability of the entity that this cursor refers to,
      * taking the current target platform into account.
      *
-     * \param cursor The cursor to query.
+     * \\param cursor The cursor to query.
      *
-     * \returns The availability of the cursor.
+     * \\returns The availability of the cursor.
+     */
+    """
+def clang_getCursorBinaryOperatorKind(arg0: CXCursor) -> CXBinaryOperatorKind:
+    """
+    /**
+     * Retrieve the binary operator kind of this cursor.
+     *
+     * If this cursor is not a binary operator then returns Invalid.
      */
     """
 def clang_getCursorCompletionString(arg0: CXCursor) -> voidp:
     """
     /**
      * Retrieve a completion string for an arbitrary declaration or macro
      * definition cursor.
      *
-     * \param cursor The cursor to query.
+     * \\param cursor The cursor to query.
      *
-     * \returns A non-context-sensitive completion string for declaration and macro
+     * \\returns A non-context-sensitive completion string for declaration and macro
      * definition cursors, or NULL for other kinds of cursors.
      */
     """
 def clang_getCursorDefinition(arg0: CXCursor) -> CXCursor:
     """
     /**
      *  For a cursor that is either a reference to or a declaration
      *  of some entity, retrieve a cursor that describes the definition of
      *  that entity.
      *
      *  Some entities can be declared multiple times within a translation
      *  unit, but only one of those declarations can also be a
      *  definition. For example, given:
      *
-     *  \code
+     *  \\code
      *  int f(int, int);
      *  int g(int x, int y) { return f(x, y); }
      *  int f(int a, int b) { return a + b; }
      *  int f(int, int);
-     *  \endcode
+     *  \\endcode
      *
      *  there are three declarations of the function "f", but only the
      *  second one is a definition. The clang_getCursorDefinition()
      *  function will take any cursor pointing to a declaration of "f"
      *  (the first or fourth lines of the example) or a cursor referenced
      *  that uses "f" (the call to "f' inside "g") and will return a
      *  declaration cursor pointing to the definition (the second "f"
@@ -9520,41 +10090,41 @@
      */
     """
 def clang_getCursorLexicalParent(arg0: CXCursor) -> CXCursor:
     """
     /**
      * Determine the lexical parent of the given cursor.
      *
-     * The lexical parent of a cursor is the cursor in which the given \p cursor
+     * The lexical parent of a cursor is the cursor in which the given \\p cursor
      * was actually written. For many declarations, the lexical and semantic parents
      * are equivalent (the semantic parent is returned by
-     * \c clang_getCursorSemanticParent()). They diverge when declarations or
+     * \\c clang_getCursorSemanticParent()). They diverge when declarations or
      * definitions are provided out-of-line. For example:
      *
-     * \code
+     * \\code
      * class C {
      *  void f();
      * };
      *
      * void C::f() { }
-     * \endcode
+     * \\endcode
      *
-     * In the out-of-line definition of \c C::f, the semantic parent is
-     * the class \c C, of which this function is a member. The lexical parent is
+     * In the out-of-line definition of \\c C::f, the semantic parent is
+     * the class \\c C, of which this function is a member. The lexical parent is
      * the place where the declaration actually occurs in the source code; in this
      * case, the definition occurs in the translation unit. In general, the
      * lexical parent for a given entity can change without affecting the semantics
      * of the program, and the lexical parent of different declarations of the
      * same entity may be different. Changing the semantic parent of a declaration,
      * on the other hand, can have a major impact on semantics, and redeclarations
      * of a particular entity should all have the same semantic context.
      *
-     * In the example above, both declarations of \c C::f have \c C as their
-     * semantic context, while the lexical context of the first \c C::f is \c C
-     * and the lexical context of the second \c C::f is the translation unit.
+     * In the example above, both declarations of \\c C::f have \\c C as their
+     * semantic context, while the lexical context of the first \\c C::f is \\c C
+     * and the lexical context of the second \\c C::f is the translation unit.
      *
      * For declarations written in the global scope, the lexical parent is
      * the translation unit.
      */
     """
 def clang_getCursorLinkage(arg0: CXCursor) -> CXLinkageKind:
     """
@@ -9577,88 +10147,88 @@
     """
 def clang_getCursorPlatformAvailability(arg0: CXCursor, arg1: int, arg2: CXString, arg3: int, arg4: CXString, arg5: CXPlatformAvailability, arg6: int) -> int:
     """
     /**
      * Determine the availability of the entity that this cursor refers to
      * on any platforms for which availability information is known.
      *
-     * \param cursor The cursor to query.
+     * \\param cursor The cursor to query.
      *
-     * \param always_deprecated If non-NULL, will be set to indicate whether the
+     * \\param always_deprecated If non-NULL, will be set to indicate whether the
      * entity is deprecated on all platforms.
      *
-     * \param deprecated_message If non-NULL, will be set to the message text
+     * \\param deprecated_message If non-NULL, will be set to the message text
      * provided along with the unconditional deprecation of this entity. The client
      * is responsible for deallocating this string.
      *
-     * \param always_unavailable If non-NULL, will be set to indicate whether the
+     * \\param always_unavailable If non-NULL, will be set to indicate whether the
      * entity is unavailable on all platforms.
      *
-     * \param unavailable_message If non-NULL, will be set to the message text
+     * \\param unavailable_message If non-NULL, will be set to the message text
      * provided along with the unconditional unavailability of this entity. The
      * client is responsible for deallocating this string.
      *
-     * \param availability If non-NULL, an array of CXPlatformAvailability instances
+     * \\param availability If non-NULL, an array of CXPlatformAvailability instances
      * that will be populated with platform availability information, up to either
      * the number of platforms for which availability information is available (as
-     * returned by this function) or \c availability_size, whichever is smaller.
+     * returned by this function) or \\c availability_size, whichever is smaller.
      *
-     * \param availability_size The number of elements available in the
-     * \c availability array.
+     * \\param availability_size The number of elements available in the
+     * \\c availability array.
      *
-     * \returns The number of platforms (N) for which availability information is
-     * available (which is unrelated to \c availability_size).
+     * \\returns The number of platforms (N) for which availability information is
+     * available (which is unrelated to \\c availability_size).
      *
      * Note that the client is responsible for calling
-     * \c clang_disposeCXPlatformAvailability to free each of the
+     * \\c clang_disposeCXPlatformAvailability to free each of the
      * platform-availability structures returned. There are
-     * \c min(N, availability_size) such structures.
+     * \\c min(N, availability_size) such structures.
      */
     """
 def clang_getCursorPrettyPrinted(arg0: CXCursor, arg1: voidp) -> CXString:
     """
     /**
      * Pretty print declarations.
      *
-     * \param Cursor The cursor representing a declaration.
+     * \\param Cursor The cursor representing a declaration.
      *
-     * \param Policy The policy to control the entities being printed. If
+     * \\param Policy The policy to control the entities being printed. If
      * NULL, a default policy is used.
      *
-     * \returns The pretty printed declaration or the empty string for
+     * \\returns The pretty printed declaration or the empty string for
      * other cursors.
      */
     """
 def clang_getCursorPrintingPolicy(arg0: CXCursor) -> voidp:
     """
     /**
      * Retrieve the default policy for the cursor.
      *
-     * The policy should be released after use with \c
+     * The policy should be released after use with \\c
      * clang_PrintingPolicy_dispose.
      */
     """
 def clang_getCursorReferenceNameRange(arg0: CXCursor, arg1: int, arg2: int) -> CXSourceRange:
     """
     /**
      * Given a cursor that references something else, return the source range
      * covering that reference.
      *
-     * \param C A cursor pointing to a member reference, a declaration reference, or
+     * \\param C A cursor pointing to a member reference, a declaration reference, or
      * an operator call.
-     * \param NameFlags A bitset with three independent flags:
+     * \\param NameFlags A bitset with three independent flags:
      * CXNameRange_WantQualifier, CXNameRange_WantTemplateArgs, and
      * CXNameRange_WantSinglePiece.
-     * \param PieceIndex For contiguous names or when passing the flag
+     * \\param PieceIndex For contiguous names or when passing the flag
      * CXNameRange_WantSinglePiece, only one piece with index 0 is
      * available. When the CXNameRange_WantSinglePiece flag is not passed for a
      * non-contiguous names, this index can be used to retrieve the individual
      * pieces of the name. See also CXNameRange_WantSinglePiece.
      *
-     * \returns The piece of the name pointed to by the given cursor. If there is no
+     * \\returns The piece of the name pointed to by the given cursor. If there is no
      * name, or if the PieceIndex is out-of-range, a null-cursor will be returned.
      */
     """
 def clang_getCursorReferenced(arg0: CXCursor) -> CXCursor:
     """
     /** For a cursor that is a reference, retrieve a cursor representing the
      * entity that it references.
@@ -9681,40 +10251,40 @@
     """
 def clang_getCursorSemanticParent(arg0: CXCursor) -> CXCursor:
     """
     /**
      * Determine the semantic parent of the given cursor.
      *
      * The semantic parent of a cursor is the cursor that semantically contains
-     * the given \p cursor. For many declarations, the lexical and semantic parents
+     * the given \\p cursor. For many declarations, the lexical and semantic parents
      * are equivalent (the lexical parent is returned by
-     * \c clang_getCursorLexicalParent()). They diverge when declarations or
+     * \\c clang_getCursorLexicalParent()). They diverge when declarations or
      * definitions are provided out-of-line. For example:
      *
-     * \code
+     * \\code
      * class C {
      *  void f();
      * };
      *
      * void C::f() { }
-     * \endcode
+     * \\endcode
      *
-     * In the out-of-line definition of \c C::f, the semantic parent is
-     * the class \c C, of which this function is a member. The lexical parent is
+     * In the out-of-line definition of \\c C::f, the semantic parent is
+     * the class \\c C, of which this function is a member. The lexical parent is
      * the place where the declaration actually occurs in the source code; in this
      * case, the definition occurs in the translation unit. In general, the
      * lexical parent for a given entity can change without affecting the semantics
      * of the program, and the lexical parent of different declarations of the
      * same entity may be different. Changing the semantic parent of a declaration,
      * on the other hand, can have a major impact on semantics, and redeclarations
      * of a particular entity should all have the same semantic context.
      *
-     * In the example above, both declarations of \c C::f have \c C as their
-     * semantic context, while the lexical context of the first \c C::f is \c C
-     * and the lexical context of the second \c C::f is the translation unit.
+     * In the example above, both declarations of \\c C::f have \\c C as their
+     * semantic context, while the lexical context of the first \\c C::f is \\c C
+     * and the lexical context of the second \\c C::f is the translation unit.
      *
      * For global declarations, the semantic parent is the translation unit.
      */
     """
 def clang_getCursorSpelling(arg0: CXCursor) -> CXString:
     """
     /**
@@ -9742,26 +10312,34 @@
      *
      * A Unified Symbol Resolution (USR) is a string that identifies a particular
      * entity (function, class, variable, etc.) within a program. USRs can be
      * compared across translation units to determine, e.g., when references in
      * one translation refer to an entity defined in another translation unit.
      */
     """
+def clang_getCursorUnaryOperatorKind(arg0: CXCursor) -> CXUnaryOperatorKind:
+    """
+    /**
+     * Retrieve the unary operator kind of this cursor.
+     *
+     * If this cursor is not a unary operator then returns Invalid.
+     */
+    """
 def clang_getCursorVisibility(arg0: CXCursor) -> CXVisibilityKind:
     """
     /**
      * Describe the visibility of the entity referred to by a cursor.
      *
      * This returns the default visibility if not explicitly specified by
      * a visibility attribute. The default visibility may be changed by
      * commandline arguments.
      *
-     * \param cursor The cursor to query.
+     * \\param cursor The cursor to query.
      *
-     * \returns The visibility of the cursor.
+     * \\returns The visibility of the cursor.
      */
     """
 def clang_getDeclObjCTypeEncoding(arg0: CXCursor) -> CXString:
     """
     /**
      * Returns the Objective-C type encoding for the specified declaration.
      */
@@ -9769,53 +10347,53 @@
 def clang_getDefinitionSpellingAndExtent(arg0: CXCursor, arg1: constcharpp, arg2: constcharpp, arg3: int, arg4: int, arg5: int, arg6: int) -> None:
     ...
 def clang_getDiagnostic(arg0: CXTranslationUnitImplp, arg1: int) -> voidp:
     """
     /**
      * Retrieve a diagnostic associated with the given translation unit.
      *
-     * \param Unit the translation unit to query.
-     * \param Index the zero-based diagnostic number to retrieve.
+     * \\param Unit the translation unit to query.
+     * \\param Index the zero-based diagnostic number to retrieve.
      *
-     * \returns the requested diagnostic. This diagnostic must be freed
-     * via a call to \c clang_disposeDiagnostic().
+     * \\returns the requested diagnostic. This diagnostic must be freed
+     * via a call to \\c clang_disposeDiagnostic().
      */
     """
 def clang_getDiagnosticCategory(arg0: voidp) -> int:
     """
     /**
      * Retrieve the category number for this diagnostic.
      *
      * Diagnostics can be categorized into groups along with other, related
      * diagnostics (e.g., diagnostics under the same warning flag). This routine
      * retrieves the category number for the given diagnostic.
      *
-     * \returns The number of the category that contains this diagnostic, or zero
+     * \\returns The number of the category that contains this diagnostic, or zero
      * if this diagnostic is uncategorized.
      */
     """
 def clang_getDiagnosticCategoryName(arg0: int) -> CXString:
     """
     /**
      * Retrieve the name of a particular diagnostic category.  This
      *  is now deprecated.  Use clang_getDiagnosticCategoryText()
      *  instead.
      *
-     * \param Category A diagnostic category number, as returned by
-     * \c clang_getDiagnosticCategory().
+     * \\param Category A diagnostic category number, as returned by
+     * \\c clang_getDiagnosticCategory().
      *
-     * \returns The name of the given diagnostic category.
+     * \\returns The name of the given diagnostic category.
      */
     """
 def clang_getDiagnosticCategoryText(arg0: voidp) -> CXString:
     """
     /**
      * Retrieve the diagnostic category text for a given diagnostic.
      *
-     * \returns The text of the given diagnostic category.
+     * \\returns The text of the given diagnostic category.
      */
     """
 def clang_getDiagnosticFixIt(arg0: voidp, arg1: int, arg2: CXSourceRange) -> CXString:
     """
     /**
      * Retrieve the replacement information for a given fix-it.
      *
@@ -9825,37 +10403,37 @@
      * the code to be removed and the replacement string is empty),
      * replacement of source code (the range covers the code to be
      * replaced and the replacement string provides the new code), and
      * insertion (both the start and end of the range point at the
      * insertion location, and the replacement string provides the text to
      * insert).
      *
-     * \param Diagnostic The diagnostic whose fix-its are being queried.
+     * \\param Diagnostic The diagnostic whose fix-its are being queried.
      *
-     * \param FixIt The zero-based index of the fix-it.
+     * \\param FixIt The zero-based index of the fix-it.
      *
-     * \param ReplacementRange The source range whose contents will be
+     * \\param ReplacementRange The source range whose contents will be
      * replaced with the returned replacement string. Note that source
      * ranges are half-open ranges [a, b), so the source code should be
      * replaced from a and up to (but not including) b.
      *
-     * \returns A string containing text that should be replace the source
-     * code indicated by the \c ReplacementRange.
+     * \\returns A string containing text that should be replace the source
+     * code indicated by the \\c ReplacementRange.
      */
     """
 def clang_getDiagnosticInSet(arg0: voidp, arg1: int) -> voidp:
     """
     /**
      * Retrieve a diagnostic associated with the given CXDiagnosticSet.
      *
-     * \param Diags the CXDiagnosticSet to query.
-     * \param Index the zero-based diagnostic number to retrieve.
+     * \\param Diags the CXDiagnosticSet to query.
+     * \\param Index the zero-based diagnostic number to retrieve.
      *
-     * \returns the requested diagnostic. This diagnostic must be freed
-     * via a call to \c clang_disposeDiagnostic().
+     * \\returns the requested diagnostic. This diagnostic must be freed
+     * via a call to \\c clang_disposeDiagnostic().
      */
     """
 def clang_getDiagnosticLocation(arg0: voidp) -> CXSourceLocation:
     """
     /**
      * Retrieve the source location of the given diagnostic.
      *
@@ -9879,46 +10457,46 @@
     """
 def clang_getDiagnosticOption(arg0: voidp, arg1: CXString) -> CXString:
     """
     /**
      * Retrieve the name of the command-line option that enabled this
      * diagnostic.
      *
-     * \param Diag The diagnostic to be queried.
+     * \\param Diag The diagnostic to be queried.
      *
-     * \param Disable If non-NULL, will be set to the option that disables this
+     * \\param Disable If non-NULL, will be set to the option that disables this
      * diagnostic (if any).
      *
-     * \returns A string that contains the command-line option used to enable this
+     * \\returns A string that contains the command-line option used to enable this
      * warning, such as "-Wconversion" or "-pedantic".
      */
     """
 def clang_getDiagnosticRange(arg0: voidp, arg1: int) -> CXSourceRange:
     """
     /**
      * Retrieve a source range associated with the diagnostic.
      *
      * A diagnostic's source ranges highlight important elements in the source
      * code. On the command line, Clang displays source ranges by
      * underlining them with '~' characters.
      *
-     * \param Diagnostic the diagnostic whose range is being extracted.
+     * \\param Diagnostic the diagnostic whose range is being extracted.
      *
-     * \param Range the zero-based index specifying which range to
+     * \\param Range the zero-based index specifying which range to
      *
-     * \returns the requested source range.
+     * \\returns the requested source range.
      */
     """
 def clang_getDiagnosticSetFromTU(arg0: CXTranslationUnitImplp) -> voidp:
     """
     /**
      * Retrieve the complete set of diagnostics associated with a
      *        translation unit.
      *
-     * \param Unit the translation unit to query.
+     * \\param Unit the translation unit to query.
      */
     """
 def clang_getDiagnosticSeverity(arg0: voidp) -> CXDiagnosticSeverity:
     """
     /**
      * Determine the severity of the given diagnostic.
      */
@@ -9983,89 +10561,100 @@
     /**
      * Retrieve the file, line, column, and offset represented by
      * the given source location.
      *
      * If the location refers into a macro expansion, retrieves the
      * location of the macro expansion.
      *
-     * \param location the location within a source file that will be decomposed
+     * \\param location the location within a source file that will be decomposed
      * into its parts.
      *
-     * \param file [out] if non-NULL, will be set to the file to which the given
+     * \\param file [out] if non-NULL, will be set to the file to which the given
      * source location points.
      *
-     * \param line [out] if non-NULL, will be set to the line to which the given
+     * \\param line [out] if non-NULL, will be set to the line to which the given
      * source location points.
      *
-     * \param column [out] if non-NULL, will be set to the column to which the given
+     * \\param column [out] if non-NULL, will be set to the column to which the given
      * source location points.
      *
-     * \param offset [out] if non-NULL, will be set to the offset into the
+     * \\param offset [out] if non-NULL, will be set to the offset into the
      * buffer to which the given source location points.
      */
     """
 def clang_getFieldDeclBitWidth(arg0: CXCursor) -> int:
     """
     /**
-     * Retrieve the bit width of a bit field declaration as an integer.
+     * Retrieve the bit width of a bit-field declaration as an integer.
+     *
+     * If the cursor does not reference a bit-field, or if the bit-field's width
+     * expression cannot be evaluated, -1 is returned.
      *
-     * If a cursor that is not a bit field declaration is passed in, -1 is returned.
+     * For example:
+     * \\code
+     * if (clang_Cursor_isBitField(Cursor)) {
+     *   int Width = clang_getFieldDeclBitWidth(Cursor);
+     *   if (Width != -1) {
+     *     // The bit-field width is not value-dependent.
+     *   }
+     * }
+     * \\endcode
      */
     """
 def clang_getFile(arg0: CXTranslationUnitImplp, arg1: str) -> voidp:
     """
     /**
      * Retrieve a file handle within the given translation unit.
      *
-     * \param tu the translation unit
+     * \\param tu the translation unit
      *
-     * \param file_name the name of the file.
+     * \\param file_name the name of the file.
      *
-     * \returns the file handle for the named file in the translation unit \p tu,
+     * \\returns the file handle for the named file in the translation unit \\p tu,
      * or a NULL file handle if the file was not a part of this translation unit.
      */
     """
 def clang_getFileContents(arg0: CXTranslationUnitImplp, arg1: voidp, arg2: int) -> str:
     """
     /**
      * Retrieve the buffer associated with the given file.
      *
-     * \param tu the translation unit
+     * \\param tu the translation unit
      *
-     * \param file the file for which to retrieve the buffer.
+     * \\param file the file for which to retrieve the buffer.
      *
-     * \param size [out] if non-NULL, will be set to the size of the buffer.
+     * \\param size [out] if non-NULL, will be set to the size of the buffer.
      *
-     * \returns a pointer to the buffer in memory that holds the contents of
-     * \p file, or a NULL pointer when the file is not loaded.
+     * \\returns a pointer to the buffer in memory that holds the contents of
+     * \\p file, or a NULL pointer when the file is not loaded.
      */
     """
 def clang_getFileLocation(arg0: CXSourceLocation, arg1: voidpp, arg2: int, arg3: int, arg4: int) -> None:
     """
     /**
      * Retrieve the file, line, column, and offset represented by
      * the given source location.
      *
      * If the location refers into a macro expansion, return where the macro was
      * expanded or where the macro argument was written, if the location points at
      * a macro argument.
      *
-     * \param location the location within a source file that will be decomposed
+     * \\param location the location within a source file that will be decomposed
      * into its parts.
      *
-     * \param file [out] if non-NULL, will be set to the file to which the given
+     * \\param file [out] if non-NULL, will be set to the file to which the given
      * source location points.
      *
-     * \param line [out] if non-NULL, will be set to the line to which the given
+     * \\param line [out] if non-NULL, will be set to the line to which the given
      * source location points.
      *
-     * \param column [out] if non-NULL, will be set to the column to which the given
+     * \\param column [out] if non-NULL, will be set to the column to which the given
      * source location points.
      *
-     * \param offset [out] if non-NULL, will be set to the offset into the
+     * \\param offset [out] if non-NULL, will be set to the offset into the
      * buffer to which the given source location points.
      */
     """
 def clang_getFileName(arg0: voidp) -> CXString:
     """
     /**
      * Retrieve the complete file and path name of the given file.
@@ -10076,19 +10665,19 @@
     /**
      * Retrieve the last modification time of the given file.
      */
     """
 def clang_getFileUniqueID(arg0: voidp, arg1: CXFileUniqueID) -> int:
     """
     /**
-     * Retrieve the unique ID for the given \c file.
+     * Retrieve the unique ID for the given \\c file.
      *
-     * \param file the file to get the ID for.
-     * \param outID stores the returned CXFileUniqueID.
-     * \returns If there was a failure getting the unique ID, returns non-zero,
+     * \\param file the file to get the ID for.
+     * \\param outID stores the returned CXFileUniqueID.
+     * \\returns If there was a failure getting the unique ID, returns non-zero,
      * otherwise returns 0.
      */
     """
 def clang_getFunctionTypeCallingConv(arg0: CXType) -> CXCallingConv:
     """
     /**
      * Retrieve the calling convention associated with a function type.
@@ -10107,15 +10696,15 @@
 def clang_getIncludedFile(arg0: CXCursor) -> voidp:
     """
     /**
      * Retrieve the file that is included by the given inclusion directive
      * cursor.
      */
     """
-def clang_getInclusions(arg0: CXTranslationUnitImplp, arg1: typing.Callable[[pylibclang._C.voidp, pylibclang._C.CXSourceLocation, int, pylibclang._C.voidp], None], arg2: voidp) -> None:
+def clang_getInclusions(arg0: CXTranslationUnitImplp, arg1: typing.Callable[[voidp, CXSourceLocation, int, voidp], None], arg2: voidp) -> None:
     """
     /**
      * Visit the set of preprocessor inclusions in a translation unit.
      *   The visitor function is called with the provided data for every included
      *   file.  This does not include headers included by the PCH file (unless one
      *   is inspecting the inclusions in the PCH file itself).
      */
@@ -10147,16 +10736,16 @@
     """
     /**
      * For reference types (e.g., "const int&"), returns the type that the
      * reference refers to (e.g "const int").
      *
      * Otherwise, returns the type itself.
      *
-     * A type that has kind \c CXType_LValueReference or
-     * \c CXType_RValueReference is a reference type.
+     * A type that has kind \\c CXType_LValueReference or
+     * \\c CXType_RValueReference is a reference type.
      */
     """
 def clang_getNullCursor() -> CXCursor:
     """
     /**
      * Retrieve the NULL cursor, which represents no entity.
      */
@@ -10210,37 +10799,37 @@
      * -1 is returned.
      */
     """
 def clang_getNumOverloadedDecls(arg0: CXCursor) -> int:
     """
     /**
      * Determine the number of overloaded declarations referenced by a
-     * \c CXCursor_OverloadedDeclRef cursor.
+     * \\c CXCursor_OverloadedDeclRef cursor.
      *
-     * \param cursor The cursor whose overloaded declarations are being queried.
+     * \\param cursor The cursor whose overloaded declarations are being queried.
      *
-     * \returns The number of overloaded declarations referenced by \c cursor. If it
-     * is not a \c CXCursor_OverloadedDeclRef cursor, returns 0.
+     * \\returns The number of overloaded declarations referenced by \\c cursor. If it
+     * is not a \\c CXCursor_OverloadedDeclRef cursor, returns 0.
      */
     """
 def clang_getOverloadedDecl(arg0: CXCursor, arg1: int) -> CXCursor:
     """
     /**
      * Retrieve a cursor for one of the overloaded declarations referenced
-     * by a \c CXCursor_OverloadedDeclRef cursor.
+     * by a \\c CXCursor_OverloadedDeclRef cursor.
      *
-     * \param cursor The cursor whose overloaded declarations are being queried.
+     * \\param cursor The cursor whose overloaded declarations are being queried.
      *
-     * \param index The zero-based index into the set of overloaded declarations in
+     * \\param index The zero-based index into the set of overloaded declarations in
      * the cursor.
      *
-     * \returns A cursor representing the declaration referenced by the given
-     * \c cursor at the specified \c index. If the cursor does not have an
+     * \\returns A cursor representing the declaration referenced by the given
+     * \\c cursor at the specified \\c index. If the cursor does not have an
      * associated set of overloaded declarations, or if the index is out of bounds,
-     * returns \c clang_getNullCursor();
+     * returns \\c clang_getNullCursor();
      */
     """
 def clang_getOverriddenCursors(arg0: CXCursor, arg1: CXCursorpp, arg2: int) -> None:
     """
     /**
      * Determine the set of methods that are overridden by the given
      * method.
@@ -10266,27 +10855,27 @@
      * a method is originally declared in a class A, then overridden in B
      * (which in inherits from A) and also in C (which inherited from B),
      * then the only overridden method returned from this function when
      * invoked on C's method will be B's method. The client may then
      * invoke this function again, given the previously-found overridden
      * methods, to map out the complete method-override set.
      *
-     * \param cursor A cursor representing an Objective-C or C++
+     * \\param cursor A cursor representing an Objective-C or C++
      * method. This routine will compute the set of methods that this
      * method overrides.
      *
-     * \param overridden A pointer whose pointee will be replaced with a
+     * \\param overridden A pointer whose pointee will be replaced with a
      * pointer to an array of cursors, representing the set of overridden
      * methods. If there are no overridden methods, the pointee will be
      * set to NULL. The pointee must be freed via a call to
-     * \c clang_disposeOverriddenCursors().
+     * \\c clang_disposeOverriddenCursors().
      *
-     * \param num_overridden A pointer to the number of overridden
+     * \\param num_overridden A pointer to the number of overridden
      * functions, will be set to the number of overridden functions in the
-     * array pointed to by \p overridden.
+     * array pointed to by \\p overridden.
      */
     """
 def clang_getPointeeType(arg0: CXType) -> CXType:
     """
     /**
      * For pointer types, returns the type of the pointee.
      */
@@ -10295,46 +10884,46 @@
     """
     /**
      * Retrieve the file, line and column represented by the given source
      * location, as specified in a # line directive.
      *
      * Example: given the following source code in a file somefile.c
      *
-     * \code
+     * \\code
      * #123 "dummy.c" 1
      *
      * static int func(void)
      * {
      *     return 0;
      * }
-     * \endcode
+     * \\endcode
      *
      * the location information returned by this function would be
      *
      * File: dummy.c Line: 124 Column: 12
      *
      * whereas clang_getExpansionLocation would have returned
      *
      * File: somefile.c Line: 3 Column: 12
      *
-     * \param location the location within a source file that will be decomposed
+     * \\param location the location within a source file that will be decomposed
      * into its parts.
      *
-     * \param filename [out] if non-NULL, will be set to the filename of the
+     * \\param filename [out] if non-NULL, will be set to the filename of the
      * source location. Note that filenames returned will be for "virtual" files,
      * which don't necessarily exist on the machine running clang - e.g. when
      * parsing preprocessed output obtained from a different environment. If
      * a non-NULL value is passed in, remember to dispose of the returned value
-     * using \c clang_disposeString() once you've finished with it. For an invalid
+     * using \\c clang_disposeString() once you've finished with it. For an invalid
      * source location, an empty string is returned.
      *
-     * \param line [out] if non-NULL, will be set to the line number of the
+     * \\param line [out] if non-NULL, will be set to the line number of the
      * source location. For an invalid source location, zero is returned.
      *
-     * \param column [out] if non-NULL, will be set to the column number of the
+     * \\param column [out] if non-NULL, will be set to the column number of the
      * source location. For an invalid source location, zero is returned.
      */
     """
 def clang_getRange(arg0: CXSourceLocation, arg1: CXSourceLocation) -> CXSourceRange:
     """
     /**
      * Retrieve a source range given the beginning and ending source
@@ -10356,31 +10945,31 @@
      */
     """
 def clang_getRemappings(arg0: str) -> voidp:
     """
     /**
      * Retrieve a remapping.
      *
-     * \param path the path that contains metadata about remappings.
+     * \\param path the path that contains metadata about remappings.
      *
-     * \returns the requested remapping. This remapping must be freed
-     * via a call to \c clang_remap_dispose(). Can return NULL if an error occurred.
+     * \\returns the requested remapping. This remapping must be freed
+     * via a call to \\c clang_remap_dispose(). Can return NULL if an error occurred.
      */
     """
 def clang_getRemappingsFromFileList(arg0: constcharpp, arg1: int) -> voidp:
     """
     /**
      * Retrieve a remapping.
      *
-     * \param filePaths pointer to an array of file paths containing remapping info.
+     * \\param filePaths pointer to an array of file paths containing remapping info.
      *
-     * \param numFiles number of file paths.
+     * \\param numFiles number of file paths.
      *
-     * \returns the requested remapping. This remapping must be freed
-     * via a call to \c clang_remap_dispose(). Can return NULL if an error occurred.
+     * \\returns the requested remapping. This remapping must be freed
+     * via a call to \\c clang_remap_dispose(). Can return NULL if an error occurred.
      */
     """
 def clang_getResultType(arg0: CXType) -> CXType:
     """
     /**
      * Retrieve the return type associated with a function type.
      *
@@ -10402,93 +10991,93 @@
      * Given a cursor that may represent a specialization or instantiation
      * of a template, retrieve the cursor that represents the template that it
      * specializes or from which it was instantiated.
      *
      * This routine determines the template involved both for explicit
      * specializations of templates and for implicit instantiations of the template,
      * both of which are referred to as "specializations". For a class template
-     * specialization (e.g., \c std::vector<bool>), this routine will return
-     * either the primary template (\c std::vector) or, if the specialization was
+     * specialization (e.g., \\c std::vector<bool>), this routine will return
+     * either the primary template (\\c std::vector) or, if the specialization was
      * instantiated from a class template partial specialization, the class template
      * partial specialization. For a class template partial specialization and a
      * function template specialization (including instantiations), this
      * this routine will return the specialized template.
      *
      * For members of a class template (e.g., member functions, member classes, or
      * static data members), returns the specialized or instantiated member.
      * Although not strictly "templates" in the C++ language, members of class
      * templates have the same notions of specializations and instantiations that
      * templates do, so this routine treats them similarly.
      *
-     * \param C A cursor that may be a specialization of a template or a member
+     * \\param C A cursor that may be a specialization of a template or a member
      * of a template.
      *
-     * \returns If the given cursor is a specialization or instantiation of a
+     * \\returns If the given cursor is a specialization or instantiation of a
      * template or a member thereof, the template or member that it specializes or
      * from which it was instantiated. Otherwise, returns a NULL cursor.
      */
     """
 def clang_getSpellingLocation(arg0: CXSourceLocation, arg1: voidpp, arg2: int, arg3: int, arg4: int) -> None:
     """
     /**
      * Retrieve the file, line, column, and offset represented by
      * the given source location.
      *
      * If the location refers into a macro instantiation, return where the
      * location was originally spelled in the source file.
      *
-     * \param location the location within a source file that will be decomposed
+     * \\param location the location within a source file that will be decomposed
      * into its parts.
      *
-     * \param file [out] if non-NULL, will be set to the file to which the given
+     * \\param file [out] if non-NULL, will be set to the file to which the given
      * source location points.
      *
-     * \param line [out] if non-NULL, will be set to the line to which the given
+     * \\param line [out] if non-NULL, will be set to the line to which the given
      * source location points.
      *
-     * \param column [out] if non-NULL, will be set to the column to which the given
+     * \\param column [out] if non-NULL, will be set to the column to which the given
      * source location points.
      *
-     * \param offset [out] if non-NULL, will be set to the offset into the
+     * \\param offset [out] if non-NULL, will be set to the offset into the
      * buffer to which the given source location points.
      */
     """
 def clang_getSymbolGraphForCursor(arg0: CXCursor) -> CXString:
     """
     /**
      * Generate a single symbol symbol graph for the declaration at the given
      * cursor. Returns a null string if the AST node for the cursor isn't a
      * declaration.
      *
      * The output contains the symbol graph as well as some additional information
      * about related symbols.
      *
-     * \param cursor the declaration for which to generate the single symbol symbol
+     * \\param cursor the declaration for which to generate the single symbol symbol
      * graph.
      *
-     * \returns a string containing the serialized symbol graph representation for
+     * \\returns a string containing the serialized symbol graph representation for
      * the symbol being queried or a null string if it can not be found in the
      * APISet.
      */
     """
 def clang_getSymbolGraphForUSR(arg0: str, arg1: CXAPISetImplp) -> CXString:
     """
     /**
      * Generate a single symbol symbol graph for the given USR. Returns a null
-     * string if the associated symbol can not be found in the provided \c CXAPISet.
+     * string if the associated symbol can not be found in the provided \\c CXAPISet.
      *
      * The output contains the symbol graph as well as some additional information
      * about related symbols.
      *
-     * \param usr is a string containing the USR of the symbol to generate the
+     * \\param usr is a string containing the USR of the symbol to generate the
      * symbol graph for.
      *
-     * \param api the \c CXAPISet to look for the symbol in.
+     * \\param api the \\c CXAPISet to look for the symbol in.
      *
-     * \returns a string containing the serialized symbol graph representation for
+     * \\returns a string containing the serialized symbol graph representation for
      * the symbol being queried or a null string if it can not be found in the
      * APISet.
      */
     """
 def clang_getTUResourceUsageName(arg0: CXTUResourceUsageKind) -> str:
     """
     /**
@@ -10504,32 +11093,32 @@
      * the template.
      *
      * This routine can be used to determine what flavor of function template,
      * class template, or class template partial specialization is stored in the
      * cursor. For example, it can describe whether a class template cursor is
      * declared with "struct", "class" or "union".
      *
-     * \param C The cursor to query. This cursor should represent a template
+     * \\param C The cursor to query. This cursor should represent a template
      * declaration.
      *
-     * \returns The cursor kind of the specializations that would be generated
-     * by instantiating the template \p C. If \p C is not a template, returns
-     * \c CXCursor_NoDeclFound.
+     * \\returns The cursor kind of the specializations that would be generated
+     * by instantiating the template \\p C. If \\p C is not a template, returns
+     * \\c CXCursor_NoDeclFound.
      */
     """
 def clang_getToken(arg0: CXTranslationUnitImplp, arg1: CXSourceLocation) -> CXToken:
     """
     /**
      * Get the raw lexical token starting with the given location.
      *
-     * \param TU the translation unit whose text is being tokenized.
+     * \\param TU the translation unit whose text is being tokenized.
      *
-     * \param Location the source location with which the token starts.
+     * \\param Location the source location with which the token starts.
      *
-     * \returns The token starting with the given location or NULL if no such token
+     * \\returns The token starting with the given location or NULL if no such token
      * exist. The returned pointer must be freed with clang_disposeTokens before the
      * translation unit is destroyed.
      */
     """
 def clang_getTokenExtent(arg0: CXTranslationUnitImplp, arg1: CXToken) -> CXSourceRange:
     """
     /**
@@ -10612,50 +11201,56 @@
     """
 def clang_getTypedefName(arg0: CXType) -> CXString:
     """
     /**
      * Returns the typedef name of the given type.
      */
     """
+def clang_getUnaryOperatorKindSpelling(arg0: CXUnaryOperatorKind) -> CXString:
+    """
+    /**
+     * Retrieve the spelling of a given CXUnaryOperatorKind.
+     */
+    """
 def clang_getUnqualifiedType(arg0: CXType) -> CXType:
     """
     /**
      * Retrieve the unqualified variant of the given type, removing as
      * little sugar as possible.
      *
      * For example, given the following series of typedefs:
      *
-     * \code
+     * \\code
      * typedef int Integer;
      * typedef const Integer CInteger;
      * typedef CInteger DifferenceType;
-     * \endcode
+     * \\endcode
      *
-     * Executing \c clang_getUnqualifiedType() on a \c CXType that
-     * represents \c DifferenceType, will desugar to a type representing
-     * \c Integer, that has no qualifiers.
+     * Executing \\c clang_getUnqualifiedType() on a \\c CXType that
+     * represents \\c DifferenceType, will desugar to a type representing
+     * \\c Integer, that has no qualifiers.
      *
-     * And, executing \c clang_getUnqualifiedType() on the type of the
+     * And, executing \\c clang_getUnqualifiedType() on the type of the
      * first argument of the following function declaration:
      *
-     * \code
+     * \\code
      * void foo(const int);
-     * \endcode
+     * \\endcode
      *
-     * Will return a type representing \c int, removing the \c const
+     * Will return a type representing \\c int, removing the \\c const
      * qualifier.
      *
      * Sugar over array types is not desugared.
      *
-     * A type can be checked for qualifiers with \c
-     * clang_isConstQualifiedType(), \c clang_isVolatileQualifiedType()
-     * and \c clang_isRestrictQualifiedType().
+     * A type can be checked for qualifiers with \\c
+     * clang_isConstQualifiedType(), \\c clang_isVolatileQualifiedType()
+     * and \\c clang_isRestrictQualifiedType().
      *
-     * A type that resulted from a call to \c clang_getUnqualifiedType
-     * will return \c false for all of the above calls.
+     * A type that resulted from a call to \\c clang_getUnqualifiedType
+     * will return \\c false for all of the above calls.
      */
     """
 def clang_hashCursor(arg0: CXCursor) -> int:
     """
     /**
      * Compute a hash value for the given cursor.
      */
@@ -10679,41 +11274,41 @@
     """
 def clang_indexSourceFile(arg0: voidp, arg1: voidp, arg2: IndexerCallbacks, arg3: int, arg4: int, arg5: str, arg6: constcharpconstp, arg7: int, arg8: CXUnsavedFile, arg9: int, arg10: CXTranslationUnitImplpp, arg11: int) -> int:
     """
     /**
      * Index the given source file and the translation unit corresponding
      * to that file via callbacks implemented through #IndexerCallbacks.
      *
-     * \param client_data pointer data supplied by the client, which will
+     * \\param client_data pointer data supplied by the client, which will
      * be passed to the invoked callbacks.
      *
-     * \param index_callbacks Pointer to indexing callbacks that the client
+     * \\param index_callbacks Pointer to indexing callbacks that the client
      * implements.
      *
-     * \param index_callbacks_size Size of #IndexerCallbacks structure that gets
+     * \\param index_callbacks_size Size of #IndexerCallbacks structure that gets
      * passed in index_callbacks.
      *
-     * \param index_options A bitmask of options that affects how indexing is
+     * \\param index_options A bitmask of options that affects how indexing is
      * performed. This should be a bitwise OR of the CXIndexOpt_XXX flags.
      *
-     * \param[out] out_TU pointer to store a \c CXTranslationUnit that can be
-     * reused after indexing is finished. Set to \c NULL if you do not require it.
+     * \\param[out] out_TU pointer to store a \\c CXTranslationUnit that can be
+     * reused after indexing is finished. Set to \\c NULL if you do not require it.
      *
-     * \returns 0 on success or if there were errors from which the compiler could
+     * \\returns 0 on success or if there were errors from which the compiler could
      * recover.  If there is a failure from which there is no recovery, returns
-     * a non-zero \c CXErrorCode.
+     * a non-zero \\c CXErrorCode.
      *
      * The rest of the parameters are the same as #clang_parseTranslationUnit.
      */
     """
 def clang_indexSourceFileFullArgv(arg0: voidp, arg1: voidp, arg2: IndexerCallbacks, arg3: int, arg4: int, arg5: str, arg6: constcharpconstp, arg7: int, arg8: CXUnsavedFile, arg9: int, arg10: CXTranslationUnitImplpp, arg11: int) -> int:
     """
     /**
      * Same as clang_indexSourceFile but requires a full command line
-     * for \c command_line_args including argv[0]. This is useful if the standard
+     * for \\c command_line_args including argv[0]. This is useful if the standard
      * library paths are relative to the binary.
      */
     """
 def clang_indexTranslationUnit(arg0: voidp, arg1: voidp, arg2: IndexerCallbacks, arg3: int, arg4: int, arg5: CXTranslationUnitImplp) -> int:
     """
     /**
      * Index the given translation unit via callbacks implemented through
@@ -10724,15 +11319,15 @@
      *
      *   -Preprocessor callbacks invocations
      *   -Declaration/reference callbacks invocations
      *   -Diagnostic callback invocations
      *
      * The parameters are the same as #clang_indexSourceFile.
      *
-     * \returns If there is a failure from which there is no recovery, returns
+     * \\returns If there is a failure from which there is no recovery, returns
      * non-zero, otherwise returns 0.
      */
     """
 def clang_index_getCXXClassDeclInfo(arg0: CXIdxDeclInfo) -> CXIdxCXXClassDeclInfo:
     ...
 def clang_index_getClientContainer(arg0: CXIdxContainerInfo) -> voidp:
     """
@@ -10815,15 +11410,15 @@
      */
     """
 def clang_isFileMultipleIncludeGuarded(arg0: CXTranslationUnitImplp, arg1: voidp) -> int:
     """
     /**
      * Determine whether the given header is guarded against
      * multiple inclusions, either with the conventional
-     * \#ifndef/\#define/\#endif macro guards or with \#pragma once.
+     * \\#ifndef/\\#define/\\#endif macro guards or with \\#pragma once.
      */
     """
 def clang_isFunctionTypeVariadic(arg0: CXType) -> int:
     """
     /**
      * Return 1 if the CXType is a variadic function type, and 0 otherwise.
      */
@@ -10838,15 +11433,15 @@
 def clang_isInvalidDeclaration(arg0: CXCursor) -> int:
     """
     /**
      * Determine whether the given declaration is invalid.
      *
      * A declaration is invalid if it could not be parsed successfully.
      *
-     * \returns non-zero if the cursor represents a declaration and it is
+     * \\returns non-zero if the cursor represents a declaration and it is
      * invalid, otherwise NULL.
      */
     """
 def clang_isPODType(arg0: CXType) -> int:
     """
     /**
      * Return 1 if the CXType is a POD (plain old data) type, and 0
@@ -10916,21 +11511,21 @@
     """
 def clang_loadDiagnostics(arg0: str, arg1: CXLoadDiag_Error, arg2: CXString) -> voidp:
     """
     /**
      * Deserialize a set of diagnostics from a Clang diagnostics bitcode
      * file.
      *
-     * \param file The name of the file to deserialize.
-     * \param error A pointer to a enum value recording if there was a problem
+     * \\param file The name of the file to deserialize.
+     * \\param error A pointer to a enum value recording if there was a problem
      *        deserializing the diagnostics.
-     * \param errorString A pointer to a CXString for recording the error string
+     * \\param errorString A pointer to a CXString for recording the error string
      *        if the file was not successfully loaded.
      *
-     * \returns A loaded CXDiagnosticSet if successful, and NULL otherwise.  These
+     * \\returns A loaded CXDiagnosticSet if successful, and NULL otherwise.  These
      * diagnostics should be released using clang_disposeDiagnosticSet().
      */
     """
 def clang_parseTranslationUnit(arg0: voidp, arg1: str, arg2: list[str], arg3: list[CXUnsavedFile], arg4: int) -> CXTranslationUnitImplp:
     ...
 def clang_parseTranslationUnit2(arg0: voidp, arg1: str, arg2: constcharpconstp, arg3: int, arg4: CXUnsavedFile, arg5: int, arg6: int, arg7: CXTranslationUnitImplpp) -> CXErrorCode:
     """
@@ -10940,71 +11535,71 @@
      *
      * This routine is the main entry point for the Clang C API, providing the
      * ability to parse a source file into a translation unit that can then be
      * queried by other functions in the API. This routine accepts a set of
      * command-line arguments so that the compilation can be configured in the same
      * way that the compiler is configured on the command line.
      *
-     * \param CIdx The index object with which the translation unit will be
+     * \\param CIdx The index object with which the translation unit will be
      * associated.
      *
-     * \param source_filename The name of the source file to load, or NULL if the
-     * source file is included in \c command_line_args.
+     * \\param source_filename The name of the source file to load, or NULL if the
+     * source file is included in \\c command_line_args.
      *
-     * \param command_line_args The command-line arguments that would be
-     * passed to the \c clang executable if it were being invoked out-of-process.
+     * \\param command_line_args The command-line arguments that would be
+     * passed to the \\c clang executable if it were being invoked out-of-process.
      * These command-line options will be parsed and will affect how the translation
      * unit is parsed. Note that the following options are ignored: '-c',
-     * '-emit-ast', '-fsyntax-only' (which is the default), and '-o \<output file>'.
+     * '-emit-ast', '-fsyntax-only' (which is the default), and '-o \\<output file>'.
      *
-     * \param num_command_line_args The number of command-line arguments in
-     * \c command_line_args.
+     * \\param num_command_line_args The number of command-line arguments in
+     * \\c command_line_args.
      *
-     * \param unsaved_files the files that have not yet been saved to disk
+     * \\param unsaved_files the files that have not yet been saved to disk
      * but may be required for parsing, including the contents of
      * those files.  The contents and name of these files (as specified by
      * CXUnsavedFile) are copied when necessary, so the client only needs to
      * guarantee their validity until the call to this function returns.
      *
-     * \param num_unsaved_files the number of unsaved file entries in \p
+     * \\param num_unsaved_files the number of unsaved file entries in \\p
      * unsaved_files.
      *
-     * \param options A bitmask of options that affects how the translation unit
+     * \\param options A bitmask of options that affects how the translation unit
      * is managed but not its compilation. This should be a bitwise OR of the
      * CXTranslationUnit_XXX flags.
      *
-     * \param[out] out_TU A non-NULL pointer to store the created
-     * \c CXTranslationUnit, describing the parsed code and containing any
+     * \\param[out] out_TU A non-NULL pointer to store the created
+     * \\c CXTranslationUnit, describing the parsed code and containing any
      * diagnostics produced by the compiler.
      *
-     * \returns Zero on success, otherwise returns an error code.
+     * \\returns Zero on success, otherwise returns an error code.
      */
     """
 def clang_parseTranslationUnit2FullArgv(arg0: voidp, arg1: str, arg2: constcharpconstp, arg3: int, arg4: CXUnsavedFile, arg5: int, arg6: int, arg7: CXTranslationUnitImplpp) -> CXErrorCode:
     """
     /**
      * Same as clang_parseTranslationUnit2 but requires a full command line
-     * for \c command_line_args including argv[0]. This is useful if the standard
+     * for \\c command_line_args including argv[0]. This is useful if the standard
      * library paths are relative to the binary.
      */
     """
 def clang_remap_dispose(arg0: voidp) -> None:
     """
     /**
      * Dispose the remapping.
      */
     """
 def clang_remap_getFilenames(arg0: voidp, arg1: int, arg2: CXString, arg3: CXString) -> None:
     """
     /**
      * Get the original and the associated filename from the remapping.
      *
-     * \param original If non-NULL, will be set to the original filename.
+     * \\param original If non-NULL, will be set to the original filename.
      *
-     * \param transformed If non-NULL, will be set to the filename that the original
+     * \\param transformed If non-NULL, will be set to the filename that the original
      * is associated with.
      */
     """
 def clang_remap_getNumFiles(arg0: voidp) -> int:
     """
     /**
      * Determine the number of remappings.
@@ -11016,89 +11611,96 @@
     """
     /**
      * Saves a translation unit into a serialized representation of
      * that translation unit on disk.
      *
      * Any translation unit that was parsed without error can be saved
      * into a file. The translation unit can then be deserialized into a
-     * new \c CXTranslationUnit with \c clang_createTranslationUnit() or,
+     * new \\c CXTranslationUnit with \\c clang_createTranslationUnit() or,
      * if it is an incomplete translation unit that corresponds to a
      * header, used as a precompiled header when parsing other translation
      * units.
      *
-     * \param TU The translation unit to save.
+     * \\param TU The translation unit to save.
      *
-     * \param FileName The file to which the translation unit will be saved.
+     * \\param FileName The file to which the translation unit will be saved.
      *
-     * \param options A bitmask of options that affects how the translation unit
+     * \\param options A bitmask of options that affects how the translation unit
      * is saved. This should be a bitwise OR of the
      * CXSaveTranslationUnit_XXX flags.
      *
-     * \returns A value that will match one of the enumerators of the CXSaveError
+     * \\returns A value that will match one of the enumerators of the CXSaveError
      * enumeration. Zero (CXSaveError_None) indicates that the translation unit was
      * saved successfully, while a non-zero value indicates that a problem occurred.
      */
     """
 def clang_sortCodeCompletionResults(arg0: CXCompletionResult, arg1: int) -> None:
     """
     /**
      * Sort the code-completion results in case-insensitive alphabetical
      * order.
      *
-     * \param Results The set of results to sort.
-     * \param NumResults The number of results in \p Results.
+     * \\param Results The set of results to sort.
+     * \\param NumResults The number of results in \\p Results.
      */
     """
 def clang_suspendTranslationUnit(arg0: CXTranslationUnitImplp) -> int:
     """
     /**
      * Suspend a translation unit in order to free memory associated with it.
      *
      * A suspended translation unit uses significantly less memory but on the other
-     * side does not support any other calls than \c clang_reparseTranslationUnit
-     * to resume it or \c clang_disposeTranslationUnit to dispose it completely.
+     * side does not support any other calls than \\c clang_reparseTranslationUnit
+     * to resume it or \\c clang_disposeTranslationUnit to dispose it completely.
      */
     """
 def clang_toggleCrashRecovery(arg0: int) -> None:
     """
     /**
      * Enable/disable crash recovery.
      *
-     * \param isEnabled Flag to indicate if crash recovery is enabled.  A non-zero
+     * \\param isEnabled Flag to indicate if crash recovery is enabled.  A non-zero
      *        value enables crash recovery, while 0 disables it.
      */
     """
 def clang_tokenize(arg0: CXTranslationUnitImplp, arg1: CXSourceRange) -> TokenArray:
     ...
 def clang_uninstall_llvm_fatal_error_handler() -> None:
     """
     /**
      * Removes currently installed error handler (if any).
      * If no error handler is intalled, the default strategy is to print error
      * message to stderr and call exit(1).
      */
     """
-def clang_visitChildren(arg0: CXCursor, arg1: typing.Callable[[pylibclang._C.CXCursor, pylibclang._C.CXCursor, pylibclang._C.voidp], CXChildVisitResult], arg2: voidp) -> int:
+def clang_visitChildren(arg0: CXCursor, arg1: typing.Callable[[CXCursor, CXCursor, voidp], CXChildVisitResult], arg2: voidp) -> int:
     """
     /**
      * Visit the children of a particular cursor.
      *
      * This function visits all the direct children of the given cursor,
-     * invoking the given \p visitor function with the cursors of each
+     * invoking the given \\p visitor function with the cursors of each
      * visited child. The traversal may be recursive, if the visitor returns
-     * \c CXChildVisit_Recurse. The traversal may also be ended prematurely, if
-     * the visitor returns \c CXChildVisit_Break.
+     * \\c CXChildVisit_Recurse. The traversal may also be ended prematurely, if
+     * the visitor returns \\c CXChildVisit_Break.
      *
-     * \param parent the cursor whose child may be visited. All kinds of
+     * \\param parent the cursor whose child may be visited. All kinds of
      * cursors can be visited, including invalid cursors (which, by
      * definition, have no children).
      *
-     * \param visitor the visitor function that will be invoked for each
-     * child of \p parent.
+     * \\param visitor the visitor function that will be invoked for each
+     * child of \\p parent.
      *
-     * \param client_data pointer data supplied by the client, which will
+     * \\param client_data pointer data supplied by the client, which will
      * be passed to the visitor each time it is invoked.
      *
-     * \returns a non-zero value if the traversal was terminated
-     * prematurely by the visitor returning \c CXChildVisit_Break.
+     * \\returns a non-zero value if the traversal was terminated
+     * prematurely by the visitor returning \\c CXChildVisit_Break.
+     */
+    """
+def clang_visitChildrenWithBlock(arg0: CXCursor, arg1: _CXChildVisitResultp) -> int:
+    """
+    /**
+     * Visits the children of a cursor using the specified block.  Behaves
+     * identically to clang_visitChildren() in all other respects.
      */
     """
```

### Comparing `pylibclang-stubs-316.0.6/pylibclang_stubs.egg-info/PKG-INFO` & `pylibclang_stubs-318.1.1/pylibclang_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibclang-stubs
-Version: 316.0.6
+Version: 318.1.1
 Summary: Python stubs for pylibclang
 License: MIT
 Project-URL: Homepage, https://github.com/edimetia3d/pylibclang
 Project-URL: Documentation, https://github.com/edimetia3d/pylibclang
 Project-URL: Repository, https://github.com/edimetia3d/pylibclang
 Project-URL: Changelog, https://github.com/edimetia3d/pylibclang/releases
 Keywords: pybind11,libclang,python,stubs
```

### Comparing `pylibclang-stubs-316.0.6/pyproject.toml` & `pylibclang_stubs-318.1.1/pyproject.toml`

 * *Files identical despite different names*

