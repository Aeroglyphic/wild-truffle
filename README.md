# wild-truffle

`wild-truffle` lets you run unpublished Truffle changes against a selection of existing commercial Truffle projects:
+ [zeppelin-solidity](https://github.com/OpenZeppelin/zeppelin-solidity/tree/7586e383c2e9d62b2f1d414e850ab365afef6d89) (at commit 7586e38)
+ [aragonOS](https://github.com/aragon/aragonOS/tree/501a90515287a8bfe015f5416e5e6aa07ced0ec4) (at commit 501a905)
+ [colonyNetwork](https://github.com/JoinColony/colonyNetwork/tree/8678f4bd7e2e93260cc40e3bdc002d8e1e3008c5) (at commit 8678f4b)

It extends Truffle's scenario testing regime to include an ~800 unit battery that reflects real usage of the toolset. 

# Use (on Travis)

Test an experimental Truffle branch (this can span across modules) against the projects listed above on Travis CI and see what breaks. (Does not require `npm install`)

```shell

git checkout -b <throw-away-branch-name>  # checkout a throw-away branch.

npm run ci <experimental-branch>          # Run the truffle branch in CI (defaults to `develop`).
```





