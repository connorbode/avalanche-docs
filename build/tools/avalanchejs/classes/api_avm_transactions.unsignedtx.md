[avalanche](../README.md) › [API-AVM-Transactions](../modules/api_avm_transactions.md) › [UnsignedTx](api_avm_transactions.unsignedtx.md)

# Class: UnsignedTx

## Hierarchy

  ↳ [StandardUnsignedTx](common_transactions.standardunsignedtx.md)‹[KeyPair](api_avm_keychain.keypair.md), [KeyChain](api_avm_keychain.keychain.md), [BaseTx](api_avm_basetx.basetx.md)›

  ↳ **UnsignedTx**

## Index

### Constructors

* [constructor](api_avm_transactions.unsignedtx.md#constructor)

### Properties

* [_codecID](api_avm_transactions.unsignedtx.md#protected-_codecid)
* [_typeID](api_avm_transactions.unsignedtx.md#protected-_typeid)
* [_typeName](api_avm_transactions.unsignedtx.md#protected-_typename)
* [codecID](api_avm_transactions.unsignedtx.md#protected-codecid)
* [transaction](api_avm_transactions.unsignedtx.md#protected-transaction)

### Methods

* [deserialize](api_avm_transactions.unsignedtx.md#deserialize)
* [fromBuffer](api_avm_transactions.unsignedtx.md#frombuffer)
* [getBurn](api_avm_transactions.unsignedtx.md#getburn)
* [getCodecID](api_avm_transactions.unsignedtx.md#getcodecid)
* [getCodecIDBuffer](api_avm_transactions.unsignedtx.md#getcodecidbuffer)
* [getInputTotal](api_avm_transactions.unsignedtx.md#getinputtotal)
* [getOutputTotal](api_avm_transactions.unsignedtx.md#getoutputtotal)
* [getTransaction](api_avm_transactions.unsignedtx.md#gettransaction)
* [getTypeID](api_avm_transactions.unsignedtx.md#gettypeid)
* [getTypeName](api_avm_transactions.unsignedtx.md#gettypename)
* [serialize](api_avm_transactions.unsignedtx.md#serialize)
* [sign](api_avm_transactions.unsignedtx.md#sign)
* [toBuffer](api_avm_transactions.unsignedtx.md#tobuffer)

## Constructors

###  constructor

\+ **new UnsignedTx**(`transaction`: [BaseTx](api_avm_basetx.basetx.md), `codecID`: number): *[UnsignedTx](api_avm_transactions.unsignedtx.md)*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[constructor](common_transactions.standardunsignedtx.md#constructor)*

*Defined in [src/common/tx.ts:289](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L289)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`transaction` | [BaseTx](api_avm_basetx.basetx.md) | undefined |
`codecID` | number | 0 |

**Returns:** *[UnsignedTx](api_avm_transactions.unsignedtx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:40](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L40)*

___

### `Protected` _typeID

• **_typeID**: *any* = undefined

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[_typeID](common_transactions.standardunsignedtx.md#protected-_typeid)*

*Defined in [src/apis/avm/tx.ts:52](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L52)*

___

### `Protected` _typeName

• **_typeName**: *string* = "UnsignedTx"

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[_typeName](common_transactions.standardunsignedtx.md#protected-_typename)*

*Defined in [src/apis/avm/tx.ts:51](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L51)*

___

### `Protected` codecID

• **codecID**: *number* = 0

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[codecID](common_transactions.standardunsignedtx.md#protected-codecid)*

*Defined in [src/common/tx.ts:199](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L199)*

___

### `Protected` transaction

• **transaction**: *[BaseTx](api_avm_basetx.basetx.md)*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[transaction](common_transactions.standardunsignedtx.md#protected-transaction)*

*Defined in [src/common/tx.ts:200](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L200)*

## Methods

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *void*

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[deserialize](common_transactions.standardunsignedtx.md#deserialize)*

*Defined in [src/apis/avm/tx.ts:56](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L56)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[fromBuffer](common_transactions.standardunsignedtx.md#abstract-frombuffer)*

*Defined in [src/apis/avm/tx.ts:66](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L66)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getBurn

▸ **getBurn**(`assetID`: Buffer): *BN*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getBurn](common_transactions.standardunsignedtx.md#getburn)*

*Defined in [src/common/tx.ts:258](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L258)*

Returns the number of burned tokens as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getCodecID](common_transactions.standardunsignedtx.md#getcodecid)*

*Overrides [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/common/tx.ts:205](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L205)*

Returns the CodecID as a number

**Returns:** *number*

___

###  getCodecIDBuffer

▸ **getCodecIDBuffer**(): *Buffer*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getCodecIDBuffer](common_transactions.standardunsignedtx.md#getcodecidbuffer)*

*Defined in [src/common/tx.ts:210](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L210)*

Returns the [Buffer](https://github.com/feross/buffer) representation of the CodecID

**Returns:** *Buffer*

___

###  getInputTotal

▸ **getInputTotal**(`assetID`: Buffer): *BN*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getInputTotal](common_transactions.standardunsignedtx.md#getinputtotal)*

*Defined in [src/common/tx.ts:219](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L219)*

Returns the inputTotal as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

###  getOutputTotal

▸ **getOutputTotal**(`assetID`: Buffer): *BN*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getOutputTotal](common_transactions.standardunsignedtx.md#getoutputtotal)*

*Defined in [src/common/tx.ts:239](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L239)*

Returns the outputTotal as a BN

**Parameters:**

Name | Type |
------ | ------ |
`assetID` | Buffer |

**Returns:** *BN*

___

###  getTransaction

▸ **getTransaction**(): *[BaseTx](api_avm_basetx.basetx.md)*

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[getTransaction](common_transactions.standardunsignedtx.md#abstract-gettransaction)*

*Defined in [src/apis/avm/tx.ts:62](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L62)*

**Returns:** *[BaseTx](api_avm_basetx.basetx.md)*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeID](common_signature.sigidx.md#gettypeid)*

*Defined in [src/utils/serialization.ts:52](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L52)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getTypeName

▸ **getTypeName**(): *string*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeName](common_signature.sigidx.md#gettypename)*

*Defined in [src/utils/serialization.ts:45](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L45)*

Used in serialization. TypeName is a string name for the type of object being output.

**Returns:** *string*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *object*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[serialize](common_transactions.standardunsignedtx.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/tx.ts:185](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L185)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  sign

▸ **sign**(`kc`: [KeyChain](api_avm_keychain.keychain.md)): *[Tx](api_avm_transactions.tx.md)*

*Overrides [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[sign](common_transactions.standardunsignedtx.md#abstract-sign)*

*Defined in [src/apis/avm/tx.ts:82](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/avm/tx.ts#L82)*

Signs this [UnsignedTx](api_avm_transactions.unsignedtx.md) and returns signed [StandardTx](common_transactions.standardtx.md)

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`kc` | [KeyChain](api_avm_keychain.keychain.md) | An [KeyChain](api_platformvm_keychain.keychain.md) used in signing  |

**Returns:** *[Tx](api_avm_transactions.tx.md)*

A signed [StandardTx](common_transactions.standardtx.md)

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [StandardUnsignedTx](common_transactions.standardunsignedtx.md).[toBuffer](common_transactions.standardunsignedtx.md#tobuffer)*

*Defined in [src/common/tx.ts:269](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L269)*

**Returns:** *Buffer*
