比特币核心整合/分期树
=====================================

[![Build Status](https://travis-ci.org/bitcoin/bitcoin.svg?branch=master)](https://travis-ci.org/bitcoin/bitcoin)

https://bitcoincore.org

什么是比特币？
----------------

比特币是实现即时付款的实验性数字货币
任何人，在世界任何地方。比特币使用点对点技术进行操作
没有中央的权力：管理交易和发行货币
由网络集体进行。 Bitcoin Core是开源的名字
可以使用这种货币的软件。

有关更多信息，以及可立即使用的二进制版本
比特币核心软件，请参阅https://bitcoin.org/en/download或阅读
[原始白皮书](https://bitcoincore.org/bitcoin.pdf)。

执照
-------

Bitcoin Core是根据MIT许可条款发布的。有关更多信息，请参见[复制](复制)
信息或查看https://opensource.org/licenses/MIT。

开发过程
-------------------

“主”分支定期建造和测试，但不能保证
完全稳定。标签(https://github.com/bitcoin/bitcoin/tags)被创建
定期发布比特币核心的官方稳定版本。

贡献工作流程在[CONTRIBUTING.md](CONTRIBUTING.md)中描述。

开发者[邮件列表](https://lists.linuxfoundation.org/mailman/listinfo/bitcoin-dev)
在工作之前应该用来讨论复杂或有争议的变化
在补丁集上。

开发者IRC可以在#bitcoin-core-dev的Freenode上找到。

测试
-------

测试和代码审查是发展的瓶颈;我们得到更多的拉
要求比我们可以在短时间内审查和测试。请耐心等待，并通过测试帮助
别人的pull请求，记住这是一个安全关键的项目，任何错误都可能导致人们的损失
很多钱。

###自动化测试

强烈建议开发人员为新代码编写[单元测试](src / test / README.md)
为旧代码提交新的单元测试。单元测试可以编译并运行
(假设它们在配置中没有被禁用)：`make check`。进一步的细节在运行
和扩展单元测试可以在[/src/test/README.md](/src/test/README.md)找到。

还有[回归和集成测试](/测试)，书面
在Python中，在构建服务器上自动运行。
这些测试可以运行(如果安装了[测试依赖关系](/ test))：`test / functional / test_runner.py`

Travis CI系统确保每个拉取请求都是为Windows，Linux和OS X构建的，并且单元/健全性测试是自动运行的。

###手动质量保证(QA)测试

更改应该由除编写该开发人员以外的人进行测试
码。这对于大的或高风险的变化尤其重要。它是有益的
如果测试更改是将测试计划添加到拉取请求描述
不直截了当

翻译
------------

可以提交对翻译的更改以及新的翻译
[比特币核心的Transifex页面](https://www.transifex.com/projects/p/bitcoin/)。

翻译定期从Transifex中提取并合并到git存储库中。看到了
[翻译过程](doc / translation_process.md)了解如何工作的细节。

**重要**：我们不接受翻译更改作为GitHub拉请求，因为下一个
从Transifex拉动会自动覆盖它们。

译员还应该订阅[邮件列表](https://groups.google.com/forum/#!forum/bitcoin-translators)。
