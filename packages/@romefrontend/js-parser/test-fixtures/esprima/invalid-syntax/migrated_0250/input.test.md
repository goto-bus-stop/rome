# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romefrontend/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > invalid-syntax > migrated_0250`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "input.js"
		end: Object {
			column: 0
			index: 37
			line: 2
		}
		start: Object {
			column: 0
			index: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: "Redefinition of __proto__ property"}
			}
			location: Object {
				filename: "input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 30
					index: 30
					line: 1
				}
				start: Object {
					column: 21
					index: 21
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "input.js"
				end: Object {
					column: 36
					index: 36
					line: 1
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
			expression: JSAssignmentExpression {
				operator: "="
				loc: Object {
					filename: "input.js"
					end: Object {
						column: 36
						index: 36
						line: 1
					}
					start: Object {
						column: 0
						index: 0
						line: 1
					}
				}
				left: JSAssignmentIdentifier {
					name: "x"
					loc: Object {
						filename: "input.js"
						identifierName: "x"
						end: Object {
							column: 1
							index: 1
							line: 1
						}
						start: Object {
							column: 0
							index: 0
							line: 1
						}
					}
				}
				right: JSObjectExpression {
					loc: Object {
						filename: "input.js"
						end: Object {
							column: 36
							index: 36
							line: 1
						}
						start: Object {
							column: 4
							index: 4
							line: 1
						}
					}
					properties: Array [
						JSObjectProperty {
							key: JSStaticPropertyKey {
								value: JSIdentifier {
									name: "__proto__"
									loc: Object {
										filename: "input.js"
										identifierName: "__proto__"
										end: Object {
											column: 15
											index: 15
											line: 1
										}
										start: Object {
											column: 6
											index: 6
											line: 1
										}
									}
								}
								loc: Object {
									filename: "input.js"
									end: Object {
										column: 15
										index: 15
										line: 1
									}
									start: Object {
										column: 6
										index: 6
										line: 1
									}
								}
							}
							value: JSNumericLiteral {
								value: 42
								format: undefined
								loc: Object {
									filename: "input.js"
									end: Object {
										column: 19
										index: 19
										line: 1
									}
									start: Object {
										column: 17
										index: 17
										line: 1
									}
								}
							}
							loc: Object {
								filename: "input.js"
								end: Object {
									column: 19
									index: 19
									line: 1
								}
								start: Object {
									column: 6
									index: 6
									line: 1
								}
							}
						}
						JSObjectProperty {
							key: JSStaticPropertyKey {
								value: JSIdentifier {
									name: "__proto__"
									loc: Object {
										filename: "input.js"
										identifierName: "__proto__"
										end: Object {
											column: 30
											index: 30
											line: 1
										}
										start: Object {
											column: 21
											index: 21
											line: 1
										}
									}
								}
								loc: Object {
									filename: "input.js"
									end: Object {
										column: 30
										index: 30
										line: 1
									}
									start: Object {
										column: 21
										index: 21
										line: 1
									}
								}
							}
							value: JSNumericLiteral {
								value: 43
								format: undefined
								loc: Object {
									filename: "input.js"
									end: Object {
										column: 34
										index: 34
										line: 1
									}
									start: Object {
										column: 32
										index: 32
										line: 1
									}
								}
							}
							loc: Object {
								filename: "input.js"
								end: Object {
									column: 34
									index: 34
									line: 1
								}
								start: Object {
									column: 21
									index: 21
									line: 1
								}
							}
						}
					]
				}
			}
		}
	]
}
```

### `diagnostics`

```

 input.js:1:21 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Redefinition of __proto__ property

    x = { __proto__: 42, __proto__: 43 }
                         ^^^^^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```