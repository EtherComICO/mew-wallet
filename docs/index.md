<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [HDWallet](#hdwallet)
    -   [getPath](#getpath)
    -   [getMnemonic](#getmnemonic)
    -   [getSeedString](#getseedstring)
    -   [getSeed](#getseed)
    -   [getChildPrivKey](#getchildprivkey)
    -   [getChildPrivKeyString](#getchildprivkeystring)
    -   [paths](#paths)
    -   [isValidMnemonic](#isvalidmnemonic)

## HDWallet

Initialize HD wallet

**Parameters**

-   `_path` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path
-   `_mneumonic` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)?** mneumonic phrase (optional, default `_mnemonic`)
-   `_password` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)?** for the mneumonic (optional, default `''`)
-   `_mnemonic`   (optional, default `bip39.generateMnemonic()`)

**Examples**

```javascript
var hd = new HDWallet("m/44'/60'/0'/0",,"test");
//returns EthereumWallet {} for ETH
```

Returns **[object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** new ethereumwallet object

### getPath

Get derivation path

Returns **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path

### getMnemonic

Get mnemonic phrase

Returns **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** mneumonic phrase

### getSeedString

Get seed string

Returns **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** returns seed as a hex string

### getSeed

Get seed

Returns **[buffer](https://nodejs.org/api/buffer.html)** returns seed as a buffer

### getChildPrivKey

Private key for specified child

**Parameters**

-   `_index` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** index of child

Returns **[buffer](https://nodejs.org/api/buffer.html)** private key

### getChildPrivKeyString

Private key for specified child

**Parameters**

-   `_index` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** index of child

Returns **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** private key

### paths

**Properties**

-   `ETH` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path for Ether.
-   `BTC` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path for Bitcoin.
-   `ETC` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path for Ether Classic.
-   `XMR` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** derivation path for Monero.

### isValidMnemonic

Validate mnemonic phrase

**Parameters**

-   `_mnemonic` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** mnemonic phrase

**Examples**

```javascript
var hd = new HDWallet("m/44'/60'/0'/0",,"test");
//returns HDWallet {} for ETH
```

Returns **[boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** true/false