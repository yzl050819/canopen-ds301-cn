# **附件A(更多信息)**
##**应用建议**
应用该协议，需要遵循以下规则以保证互操作性。这些规则包括下列方面：
##**1 无效COB’s**
如果一个COB的COB-ID遵守协议规范，但根据协议规范它包含无效的参数值，那么它就是无效的。这可能由于低层的错误或应用错误造成，无效COB’s需由上层应用处理而不在本文范围，而无效COB应被协议栈忽略。
##**2 Time-out's**
由于COB’s可能被忽略，应答确认可能永远也不能到达。要解决这种问题，就需要在一定的时间后通知用户(time-out)。超时并不算对服务的确认。超时表示该服务尚未完成。由应用程序应该处理这种状况。 超时时间由具体应用指定，因而不属于本规范的范围。然而，推荐具体应用能够提供修改超时时间的工具以满足要求。
##**3 PDO传输类型 0、254、255**
如果在相应协议中未特别规定，传输类型254和255的PDOs在设备进入运行态后直接发送，而类型 0还要收到一条Sync。
##**4 对象字典通信对象总览**
略

