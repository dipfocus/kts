## 访问KTS
KTS是一种Web服务，Region是指金山云服务的服务区，一般以地域作为划分单位。Endpoint是访问KTS服务的一个url，例如：http://kts.cn-beijing-1.ksyun.com 是访问北京Region1的KTS服务的url入口。该服务目前使用HTTP进行传输，使用protobuf作为消息序列化格式。您的应用程序代码可以直接向KTS服务API发送请求，但是我们建议使用KTS的SDK，而不是直接从应用程序对KTS API发请求。目前KTS服务提供了Java语言的SDK，另外我们还提供管理控制台，让您能够处理表的相关管理类操作。  
KTS使用Credentials对请求进行身份认证和鉴权，每个合法的KTS请求都必须携带正确的Credentials信息。Credentials有AccessKey和SecretKey组成，AccessKey用于标识Credentials，SecretKey用于加密KTS请求。SecretKey是认证请求身份的重要凭证，因此需要保证SecretKey的保密和安全。用户可以在金山云官网的用户中心管理自己的AccessKey和SecretKey。
