# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `typescript > types > function-with-this`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "typescript/types/function-with-this/input.ts"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "module"
	syntax: Array ["ts"]
	loc: Object {
		filename: "typescript/types/function-with-this/input.ts"
		end: Object {
			column: 0
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	body: Array [
		JSVariableDeclarationStatement {
			loc: Object {
				filename: "typescript/types/function-with-this/input.ts"
				end: Object {
					column: 30
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			declaration: JSVariableDeclaration {
				kind: "let"
				loc: Object {
					filename: "typescript/types/function-with-this/input.ts"
					end: Object {
						column: 30
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				declarations: Array [
					JSVariableDeclarator {
						id: JSBindingIdentifier {
							name: "f"
							loc: Object {
								filename: "typescript/types/function-with-this/input.ts"
								end: Object {
									column: 29
									line: 1
								}
								start: Object {
									column: 4
									line: 1
								}
							}
							meta: JSPatternMeta {
								definite: undefined
								loc: Object {
									filename: "typescript/types/function-with-this/input.ts"
									end: Object {
										column: 29
										line: 1
									}
									start: Object {
										column: 4
										line: 1
									}
								}
								typeAnnotation: TSFunctionType {
									loc: Object {
										filename: "typescript/types/function-with-this/input.ts"
										end: Object {
											column: 29
											line: 1
										}
										start: Object {
											column: 7
											line: 1
										}
									}
									typeAnnotation: TSVoidKeywordTypeAnnotation {
										loc: Object {
											filename: "typescript/types/function-with-this/input.ts"
											end: Object {
												column: 29
												line: 1
											}
											start: Object {
												column: 25
												line: 1
											}
										}
									}
									meta: TSSignatureDeclarationMeta {
										rest: undefined
										typeParameters: undefined
										loc: Object {
											filename: "typescript/types/function-with-this/input.ts"
											end: Object {
												column: 29
												line: 1
											}
											start: Object {
												column: 7
												line: 1
											}
										}
										parameters: Array [
											JSBindingIdentifier {
												name: "this"
												loc: Object {
													filename: "typescript/types/function-with-this/input.ts"
													identifierName: "this"
													end: Object {
														column: 12
														line: 1
													}
													start: Object {
														column: 8
														line: 1
													}
												}
												meta: JSPatternMeta {
													optional: undefined
													loc: Object {
														filename: "typescript/types/function-with-this/input.ts"
														end: Object {
															column: 20
															line: 1
														}
														start: Object {
															column: 8
															line: 1
														}
													}
													typeAnnotation: TSNumberKeywordTypeAnnotation {
														loc: Object {
															filename: "typescript/types/function-with-this/input.ts"
															end: Object {
																column: 20
																line: 1
															}
															start: Object {
																column: 14
																line: 1
															}
														}
													}
												}
											}
										]
									}
								}
							}
						}
						init: undefined
						loc: Object {
							filename: "typescript/types/function-with-this/input.ts"
							end: Object {
								column: 29
								line: 1
							}
							start: Object {
								column: 4
								line: 1
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
✔ No known problems!

```
