# go build ./... bug

### Instructions
1. `$ git clone git@github.com:xyzst/go-build-bug.git`
2. `$ cd go-build-bug`
3. `$ git checkout aa17a6c192c112d61929c87412c96f741156de96`
4. `$ cd L1/M0`
5. `$ go build ./...` (✅ generates a binary/executable named "build-bug" as expected)
6. `$ ./build-bug` 
    ```
    2020/06/10 19:40:37 Hello from Austin, TX!
    ```
7. `$ git checkout 29666294d9f29f2e9b8f237f885402ace41c6103`
8. `$ go build ./...` (❌ does not generate new binary/executable, text should be reversed in the next step)
9. `$ ./build-bug` 
   ```
   2020/06/10 19:41:49 Hello from Austin, TX!
   ```
