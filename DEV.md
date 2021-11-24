## 合约仓库:
https://github.com/KAFKA-PROTOCOL/dev-contracts

## SDK仓库
https://github.com/KAFKA-PROTOCOL/dev-sdk

## 前端仓库
https://github.com/KAFKA-PROTOCOL/dev-interface

### 前端编译步骤
#### 1. 编译SDK
下载SDK仓库，安装依赖并编译
#### 2. 链接SDK到前端仓库
将SDK编译出的dist文件夹复制或者链接到前端库中的 node_modules/@uniswap/sdk/dist
#### 3. 修改DEFAULT_TOKEN_LIST
将node_modules/@uniswap/default-token-list/build/uniswap-default.tokenlist.json 内容替换为 https://github.com/KAFKA-PROTOCOL/dev-contracts/blob/fdr/cocoSwap_525.json
#### 4. 编译
`yarn build` & `yarn start`

### 前端已做的修改
大部分修改搜索`ChainId.LOCAL`可找到。

### METAMASK对接
安装metamask, 并添加自定义网络:
```
rpc: https://prod-forge.prod.findora.org:8545
chainId: 525
block explorer: http://blockscout.findorascan.io/
```