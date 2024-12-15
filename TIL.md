# [How to Test Conflating Stateflow](https://zsmb.co/conflating-stateflows/)
###### Date: 2024/12/15

Separate assert and code triggering into 2 different set of `coroutine launch`
* the first one is for assertion, the launch should use `UnconfinedTestDispatcher`
* the other (last) one is for trigger the code / sequence / logic

Please note that when using flow the code triggering should still use a separate launch and not inside the `test` block

---