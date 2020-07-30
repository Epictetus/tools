# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/js-parser/index.test.ts --update-snapshots` to update.

## `experimental > class-private-properties > failure-computed`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "experimental/class-private-properties/failure-computed/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "experimental/class-private-properties/failure-computed/input.js"
		end: Object {
			column: 0
			index: 34
			line: 5
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
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Expected an identifier"}]}
			}
			location: Object {
				filename: "experimental/class-private-properties/failure-computed/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 3
					index: 24
					line: 3
				}
				start: Object {
					column: 3
					index: 24
					line: 3
				}
			}
		}
	]
	body: Array [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "Foo"
				loc: Object {
					filename: "experimental/class-private-properties/failure-computed/input.js"
					identifierName: "Foo"
					end: Object {
						column: 9
						index: 9
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
				filename: "experimental/class-private-properties/failure-computed/input.js"
				end: Object {
					column: 1
					index: 33
					line: 4
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
			meta: JSClassHead {
				implements: undefined
				superClass: undefined
				superTypeParameters: undefined
				typeParameters: undefined
				loc: Object {
					filename: "experimental/class-private-properties/failure-computed/input.js"
					end: Object {
						column: 1
						index: 33
						line: 4
					}
					start: Object {
						column: 0
						index: 0
						line: 1
					}
				}
				body: Array [
					JSClassPrivateProperty {
						key: JSPrivateName {
							id: JSIdentifier {
								name: "p"
								loc: Object {
									filename: "experimental/class-private-properties/failure-computed/input.js"
									identifierName: "p"
									end: Object {
										column: 4
										index: 16
										line: 2
									}
									start: Object {
										column: 3
										index: 15
										line: 2
									}
								}
							}
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								end: Object {
									column: 4
									index: 16
									line: 2
								}
								start: Object {
									column: 2
									index: 14
									line: 2
								}
							}
						}
						value: JSReferenceIdentifier {
							name: "x"
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								identifierName: "x"
								end: Object {
									column: 8
									index: 20
									line: 2
								}
								start: Object {
									column: 7
									index: 19
									line: 2
								}
							}
						}
						typeAnnotation: undefined
						loc: Object {
							filename: "experimental/class-private-properties/failure-computed/input.js"
							end: Object {
								column: 8
								index: 20
								line: 2
							}
							start: Object {
								column: 2
								index: 14
								line: 2
							}
						}
						meta: JSClassPropertyMeta {
							abstract: false
							accessibility: undefined
							optional: false
							readonly: false
							static: false
							typeAnnotation: undefined
							start: Object {
								column: 2
								index: 14
								line: 2
							}
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								end: Object {
									column: 4
									index: 16
									line: 2
								}
								start: Object {
									column: 2
									index: 14
									line: 2
								}
							}
						}
					}
					JSClassProperty {
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: ""
								loc: Object {
									filename: "experimental/class-private-properties/failure-computed/input.js"
									identifierName: ""
									end: Object {
										column: 6
										index: 27
										line: 3
									}
									start: Object {
										column: 5
										index: 26
										line: 3
									}
								}
							}
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								end: Object {
									column: 6
									index: 27
									line: 3
								}
								start: Object {
									column: 5
									index: 26
									line: 3
								}
							}
						}
						value: JSNumericLiteral {
							value: 1
							format: undefined
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								end: Object {
									column: 10
									index: 31
									line: 3
								}
								start: Object {
									column: 9
									index: 30
									line: 3
								}
							}
						}
						definite: undefined
						typeAnnotation: undefined
						loc: Object {
							filename: "experimental/class-private-properties/failure-computed/input.js"
							end: Object {
								column: 10
								index: 31
								line: 3
							}
							start: Object {
								column: 5
								index: 26
								line: 3
							}
						}
						meta: JSClassPropertyMeta {
							abstract: false
							accessibility: undefined
							optional: false
							readonly: false
							static: false
							typeAnnotation: undefined
							start: Object {
								column: 5
								index: 26
								line: 3
							}
							loc: Object {
								filename: "experimental/class-private-properties/failure-computed/input.js"
								end: Object {
									column: 6
									index: 27
									line: 3
								}
								start: Object {
									column: 5
									index: 26
									line: 3
								}
							}
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 experimental/class-private-properties/failure-computed/input.js:3:3 parse/js ━━━━━━━━━━━━━━━━━━━━━━

  ✖ Expected an identifier

    1 │ class Foo {
    2 │   #p = x
  > 3 │   #[m] = 1
      │    ^
    4 │ }

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```