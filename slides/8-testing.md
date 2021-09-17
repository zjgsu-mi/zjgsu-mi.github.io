---
author: 韩建伟
title:  "软件测试"
date:   2021-09-18
---

# [软件测试][software-testing]

- 现代软件开发中非常重要的一个环节
- 保证软件质量的重要手段
- [Awesome Software Quality][]

# 单元测试

- 保证代码片段的正确性
- 通常是对函数进行测试
- 写程序之前应先写好代码的单元测试
- 每次修改程序后运行单元测试以保证代码的正确性
- [TDD（测试驱动开发）][tdd]

# 单元测试工具

- Python: [nose][]、[unittest][]
- Java: [JUnit][]
- JavaScript: [mocha][]、[jest][]

# 自动化测试

- 使用特定软件来执行测试流程
- 比较实际结果与预期结果之间的差异
- 参考[Awesome Test Automation][]来帮助实现测试自动化
- [持续集成][ci]中非常重要的组成部分

[awesome software quality]: https://github.com/ligurio/awesome-software-quality
[awesome test automation]: https://github.com/atinfo/awesome-test-automation
[ci]: http://www.ruanyifeng.com/blog/2015/09/continuous-integration.html
[jest]: https://github.com/facebook/jest
[junit]: http://junit.org/
[mocha]: https://github.com/mochajs/mocha
[nose]: https://github.com/nose-devs/nose
[software-testing]: https://zh.wikipedia.org/wiki/%E8%BD%AF%E4%BB%B6%E6%B5%8B%E8%AF%95
[tdd]: https://github.com/unicodeveloper/awesome-tdd
[unittest]: https://docs.python.org/3/library/unittest.html
