See also http://pvp.haskell.org/faq

#### 0.1.6.3

* Test-suite: add dependency `attoparsec-aeson` for `aeson-2.2`.

Tested with GHC 8.0 - 9.8.

#### 0.1.6.2

* Allow `mtl-2.3` (no code change).
* Run test-suite via `cabal test`.

Tested with GHC 7.4 - 9.6.

#### 0.1.6.1 revision 1

* Allow `text-2.0` (no code change).

#### 0.1.6.1

* Build with GHC 9.2 and `ghc-prim-0.8` (via `base-4.16`).

### 0.1.6.0

* New function `openConnectionAddress''` supporting supplying local `SSLContext`s as well as modifying the `SSL` connection before initiating the client SSL handshake.
* New function `openConnectionSSL'` which allows to customize the SSL connection _before_ a client SSL handshake is attempted.
* New convenience function `getContextSSL` function allowing to retrieve global `SSLContext`.

### 0.1.5.0

* New function `openConnectionAddress'` function supporting supplying local `SSLContext`s.

### 0.1.4.0

* New module `Network.Http.Client.WebSocket` providing basic RFC6455 support.
* New function `inputStreamBodyChunked` supporting breaking up over-sized chunks.

### 0.1.3.0

* New functions `receiveUpgradeResponse`, `receiveConnectResponse`, and `unsafeWithRawStreams` for accessing full-duplex low-level streams (e.g. for upgrading to Websockets protocol).
* New function `makeConnection` for constructing a `Connection` object over custom streams.

### 0.1.2.0

* New functions `unsafeReceiveResponse` and `unsafeReceiveResponseRaw` that do not automatically skip to end-of-stream.

### 0.1.1.0

* New alternative connection-setup API (`ConnectionAddress` et al.).
* New function `getHeaderMap` for exporting all response headers at once.
* Add convenience functions `bytestringBody`, `lazyBytestringBody`, `utf8TextBody`, `utf8LazyTextBody`.
* Add support for Brotli HTTP compression.

## 0.1.0.0

* First version. Released on an unsuspecting world.
* Derived from `http-streams-core-0.8.6.1` & `http-common-0.8.2.0`.
