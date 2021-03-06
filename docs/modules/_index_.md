[randomify - v1.3.2](../README.md) › [Globals](../globals.md) › ["index"](_index_.md)

# External module: "index"

## Index

### Functions

* [join](_index_.md#const-join)
* [pick](_index_.md#const-pick)
* [pickString](_index_.md#const-pickstring)
* [randint](_index_.md#const-randint)
* [random](_index_.md#const-random)
* [randomColor](_index_.md#const-randomcolor)
* [range](_index_.md#const-range)

## Functions

### `Const` join

▸ **join**<**T**>(`array`: T[], `separator`: string | function): *string*

*Defined in [index.ts:6](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L6)*

Join an array with a function or string.

**Type parameters:**

▪ **T**

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`array` | T[] | - | The array to be joined. |
`separator` | string &#124; function | "," | The separator to be put inbetween the elements in the array. Can be a string or a function.  |

**Returns:** *string*

___

### `Const` pick

▸ **pick**<**T**>(`array`: T[]): *T*

*Defined in [index.ts:18](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L18)*

```ts
const coinFlip = pick(["Tails!", "Heads!"])
```
Pick a random element from an array.

**Type parameters:**

▪ **T**

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`array` | T[] | The array that the element is going to be picked from.  |

**Returns:** *T*

___

### `Const` pickString

▸ **pickString**(`str`: string, `len`: number): *string*

*Defined in [index.ts:56](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L56)*

Get a random string from a set of characters.
```ts
const ID = pickString("0123456789abcdefABCDEF", 12) // A possible return is "bB0d4D840bfc"
```

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`str` | string | - | The set of characters that the generated string will be picked from. |
`len` | number |  str.length | The length of the generated string.  |

**Returns:** *string*

___

### `Const` randint

▸ **randint**(`min`: number, `max`: number, `decimals`: boolean): *number*

*Defined in [index.ts:38](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L38)*

```ts
randint(1, 5) // 1, 2, 3, 4
randint(1, 5, true) // Any float between 1 and 5.
```
Returns a random integer from min to max, but never reaching max.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`min` | number | - | The minimum value. |
`max` | number | - | The maximum value. |
`decimals` | boolean | false | Whether to have decimals in the output.  |

**Returns:** *number*

___

### `Const` random

▸ **random**(`strings`: TemplateStringsArray, ...`added`: any[]): *string*

*Defined in [index.ts:27](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L27)*

```ts
random`It is currently ${["daytime", "nighttime", "afternoon"]}. It's time to ${["work", "exercise", "eat"]}!`
```
A template literal tag that chooses random elements from its placeholders.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`strings` | TemplateStringsArray | The strings from the template literal. |
`...added` | any[] | The placeholders. They can be either "any" or an array. If it's an array, it will pick a random element from it.  |

**Returns:** *string*

___

### `Const` randomColor

▸ **randomColor**(): *string*

*Defined in [index.ts:60](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L60)*

**Returns:** *string*

___

### `Const` range

▸ **range**(`min`: number, `max`: number): *number[]*

*Defined in [index.ts:47](https://github.com/TNThacker2015/randomify/blob/9197677/src/index.ts#L47)*

```ts
range(1, 7) // [1, 2, 3, 4, 5, 6]
```
Gets a list with values ranging from the min value to max value, excluding the max value.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`min` | number | The minimum value. |
`max` | number | The maximum value.  |

**Returns:** *number[]*
