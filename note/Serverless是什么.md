Serverless架构即事件驱动的架构；

Serverless架构或者Serverless工程的核心思想是函数即服务；从技术角度来讲，互联网上最准确的“Serverless计算”的定义如下：

“Serverless计算又称为函数即服务（FAAS），它是一种云计算和代码执行模型，其中云提供商管理函数的容器——平台即服务（PaaS）——的启动和停止。”

“函数即服务”意味着任何Serverless模型都有一个在云平台上运行的函数；这些函数只不过是代码块，它们的执行取决于与之相关联的触发器。

数启动和停止的管理机制：只要有触发器触发了某个函数，云平台就会启动一个容器，用来执行该函数；一旦该函数执行成功并返回结果，或者运行超时，那么运行该函数的容器就将被云平台回收或者销毁；在高负载的情况下，或者当两个触发器之间几乎不存在时间间隔时，这种回收机制使得容器能够被重复利用。

因此，我们可以明确地指出，对于采用Serverless架构的应用程序，其服务器不会一直运行。其好处显而易见，那就是无须专门的运维团队成员来维护和管理服务器。节省出来的人力可以专注于其他事情，比如软件研发等。同时，这也为公司和个人节省了资源和成本。对于那些经常使用GPU实例应对高负载的机器学习和数据工程团队来说，好处就更加明显了。因此，按需运行的Serverless GPU实例无须开发人员或者运维团队全天候维护，从而能够节省一大笔资金。