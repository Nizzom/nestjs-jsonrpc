# NestJS JSON RPC package - [nestjs-json-rpc-httpstatus](https://www.npmjs.com/package/nestjs-json-rpc-httpstatus) npm package

## This package was forked from [nestjs-json-rpc](https://www.npmjs.com/package/@jashkasoft/nestjs-json-rpc) package repo, only sending http status codes on error has been implemented

Implemented JSON RPC [specification](https://www.jsonrpc.org/specification)

### Custom Exception

```typescript
import { RpcException } from 'nestjs-json-rpc-httpstatus';

export class MyRpcException extends RpcException {
  constructor(message: string | object, code: number) {
    super(message, code);
  }
}
```

RpcException returns 500

RpcInternalException returns 500

RpcInvalidParamsException returns 500

RpcInvalidRequestException returns 400

RpcMethodNotFoundException returns 404


## See full doc [nestjs-json-rpc](https://www.npmjs.com/package/@jashkasoft/nestjs-json-rpc)
