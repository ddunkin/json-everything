# [1.6.0](https://github.com/gregsdennis/json-everything/pull/130)

[#128](https://github.com/gregsdennis/json-everything/pull/128) - Added support for nullability.  Special thanks to [@JMPSequeira](https://github.com/JMPSequeira) who proposed the feature and worked through multiple designs ([#124](https://github.com/gregsdennis/json-everything/pull/124) and [#127](https://github.com/gregsdennis/json-everything/pull/127)) that lead to the final solution and for adding all the tests needed to ensure proper function.
- Added `NullableAttribute`.
- Added `Nullability`.
- Added `SchemaGenerationConfiguration.Nullability`.

[#125](https://github.com/gregsdennis/json-everything/pull/125) - Bug fix: generation of object with no serializable properties still generates an empty `properties` keyword.

Also updated intent classes to be mutable.  Should have been this way to begin with, but was probably an oversight.

# [1.5.0](https://github.com/gregsdennis/json-everything/pull/115)

[#114](https://github.com/gregsdennis/json-everything/issues/114) - `DateTime` properties not generating properly.  Also fixes `Guid`, `JsonPointer`, and  `Uri` properties.

Added `PropertyNamesIntent`.

# [1.4.0](https://github.com/gregsdennis/json-everything/pull/113)

[#109](https://github.com/gregsdennis/json-everything/issues/109) - Add properties in the order they're declared in code.  Credit to [@wazzamatazz](https://github.com/jaysvoboda)

[#112](https://github.com/gregsdennis/json-everything/issues/112) - Add properties in the order they're declared in code.

# [1.3.2](https://github.com/gregsdennis/json-everything/pull/105)

Fixes property name callout in `required` keyword.  Credit to [@jaysvoboda](https://github.com/jaysvoboda) for finding and fixing this.

# [1.3.1](https://github.com/gregsdennis/json-everything/pull/101)

[#100](https://github.com/gregsdennis/json-everything/issues/100) - Don't optimize type-only subschemas.

# [1.3.0](https://github.com/gregsdennis/json-everything/pull/98)

[#96](https://github.com/gregsdennis/json-everything/issues/96) - Added `ISchemaRefiner` to the schema generation process to allow users to inject custom logic after intents are created.

[#97](https://github.com/gregsdennis/json-everything/issues/97) - Fixed an issue with subsequent schema generations off of the same type.

# [1.2.3](https://github.com/gregsdennis/json-everything/pull/88)

[#87](https://github.com/gregsdennis/json-everything/issues/87) - Generation for the same property type under different property names causes StackOverflowException.

# [1.2.2](https://github.com/gregsdennis/json-everything/pull/86)

[#85](https://github.com/gregsdennis/json-everything/issues/85) - Generation for `List<TSelf>` producing StackOverflowException.

# [1.2.1](https://github.com/gregsdennis/json-everything/pull/75)

Added support for nullable reference types.

# [1.2.0](https://github.com/gregsdennis/json-everything/pull/74)

Added support for .Net 5 and remaining in-built JSON serialization attributes: `JsonInclude` & `JsonNumberHandling`.

Exposed static class `AttributeHandler` and added methods to allow for handlers of predefined attributes.  This mechanism should only be used for attributes that cannot also be made to implement `IAttributeHandler`.  Attributes which also implement this interface are implicitly handled.

# [1.1.1](https://github.com/gregsdennis/json-everything/pull/61)

Signed the DLL for strong name compatibility.

# [1.1.0](https://github.com/gregsdennis/json-everything/pull/49)

Added support for in-built JSON serialization attributes (Standard 2.0 & Core 3.x): `JsonPropertyName` & `JsonIgnore`.

# [1.0.1](https://github.com/gregsdennis/json-everything/pull/45)

Added debug symbols to package.  No functional change.

# [1.0.0](https://github.com/gregsdennis/json-everything/pull/41)

Initial release.