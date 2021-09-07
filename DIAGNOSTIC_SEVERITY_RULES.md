Diagnostic Severity Rules
=====================
This doc details all available rules that can be customized using the `python.analysis.diagnosticSeverityOverrides` setting. If you are looking for details on other available settings, please refer back to the main [README](README.md).

| Value  | Description                                                                                                               |
|--------|---------------------------------------------------------------------------------------------------------------------------|
| reportGeneralTypeIssues | Diagnostics for general type inconsistencies, unsupported operations, argument/parameter mismatches, etc. This covers all of the basic type-checking rules not covered by other rules. It does not include syntax errors. |
| reportPropertyTypeMismatch | Diagnostics for properties where the type of the value passed to the setter is not assignable to the value returned by the getter. Such mismatches violate the intended use of properties, which are meant to act like variables. |
| reportFunctionMemberAccess | Diagnostics for member accesses on functions. |
| reportMissingImports | Diagnostics for imports that have no corresponding imported python file or type stub file. |
dfsdfsdfdsf
| reportUnusedFunction | Diagnostics for a function or method with a private name (starting with an underscore) that is not accessed. |
| reportUnusedVariable | Diagnostics for a variable that is not accessed. |
| reportDuplicateImport | Diagnostics for an imported symbol or module that is imported more than once. |
| reportWildcardImportFromLibrary | Diagnostics for an wildcard import from an external library. |
| reportOptionalSubscript | Diagnostics for an attempt to subscript (index) a variable with an Optional type. |
| reportOptionalMemberAccess | Diagnostics for an attempt to access a member of a variable with an Optional type. |
| reportOptionalCall | Diagnostics for an attempt to call a variable with an Optional type. |
| reportOptionalIterable | Diagnostics for an attempt to use an Optional type as an iterable value (e.g. within a for statement). |
| reportOptionalContextManager | Diagnostics for an attempt to use an Optional type as a context manager (as a parameter to a with statement). |
| reportOptionalOperand | Diagnostics for an attempt to use an Optional type as an operand to a binary or unary operator (like '+', '==', 'or', 'not'). |
| reportTypedDictNotRequiredAccess | Diagnostics for an attempt to access a non-required key within a TypedDict without a check for its presence. |
| reportUntypedFunctionDecorator | Diagnostics for function decorators that have no type annotations. These obscure the function type, defeating many type analysis features.  |
| reportUntypedClassDecorator | Diagnostics for class decorators that have no type annotations. These obscure the class type, defeating many type analysis features. |
| reportUntypedBaseClass | Diagnostics for base classes whose type cannot be determined statically. These obscure the class type, defeating many type analysis features. |
| reportUntypedNamedTuple | Diagnostics when “namedtuple” is used rather than “NamedTuple”. The former contains no type information, whereas the latter does. |
| reportPrivateUsage | Diagnostics for incorrect usage of private or protected variables or functions. Protected class members begin with a single underscore `_` and can be accessed only by subclasses. Private class members begin with a double underscore but do not end in a double underscore and can be accessed only within the declaring class. Variables and functions declared outside of a class are considered private if their names start with either a single or double underscore, and they cannot be accessed outside of the declaring module. |
| reportConstantRedefinition | Diagnostics for attempts to redefine variables whose names are all-caps with underscores and numerals. |
| reportIncompatibleMethodOverride | Diagnostics for methods that override a method of the same name in a base class in an incompatible manner (wrong number of parameters, incompatible parameter types, or incompatible return type). |
| reportIncompatibleVariableOverride | Diagnostics for class variable declarations that override a symbol of the same name in a base class with a type that is incompatible with the base class symbol type. |
| reportOverlappingOverload | Diagnostics for function overloads that overlap in signature and obscure each other or have incompatible return types. |
| reportInvalidStringEscapeSequence | Diagnostics for invalid escape sequences used within string literals. The Python specification indicates that such sequences will generate a syntax error in future versions. |
| reportUnknownParameterType | Diagnostics for input or return parameters for functions or methods that have an unknown type. |
| reportUnknownArgumentType | Diagnostics for call arguments for functions or methods that have an unknown type. |
| reportUnknownLambdaType | Diagnostics for input or return parameters for lambdas that have an unknown type. |
| reportUnknownVariableType | Diagnostics for variables that have an unknown type.  |
| reportUnknownMemberType | Diagnostics for class or instance variables that have an unknown type. |
sfsdf
