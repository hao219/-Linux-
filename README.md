项目名称：{面向Linux内核的高效地址空间隔离} 

项目链接：{https://github.com/hao219/-Linux-?tab=readme-ov-file#-linux-}

导师信息：{樊浩，haofan@hust.edu.cn}

难度：{高}

分类：{新型内核 }

题目要求：{Linux内核运行在内核地址空间，管理所有的硬件， 并有权限访问所有的内存，每一个用户态应用通过系统调用进入内核后都会访问统一的内核视图，即容器间共享内核的代码与数据。这种设计会在云原生等多用户并发场景中导致安全性问题。Linux 内核中现有的容器级语义：CGroup、 NameSpace 等等过于薄弱，没有深入系统核心底层，因此这些机制能力有限，例如：CGroup可以限制内存使用量，但是无法限制内存恶意访问。现有的内存隔离方法无法和共享内核有效统一，不能有效平衡性能、系统兼容性和应用适配性。从内核页表机制出发，设计高效的内核地址空间隔离方法，在不产生明显性能损失的前提下实现数据隔离架构，并在此架构基础上进行若干种类数据的隔离。}

特征：{}

预期目标：{
1.从内核页表机制出发，设计高效的内核地址空间隔离方法，在不产生明显性能损失的前提下实现数据隔离架构
2.在此架构基础上进行若干种类数据的隔离
}

License：{}

参考资料：{Xia, H., Zhang, D., Liu, W., Haller, I., Sherwin, B., & Chisnall, D. (2022, May). A secret-free hypervisor: Rethinking isolation in the age of speculative vulnerabilities. In 2022 IEEE Symposium on Security and Privacy (SP) (pp. 370-385). IEEE.

Behrens, J., Cao, A., Skeggs, C., Belay, A., Kaashoek, M. F., & Zeldovich, N. (2020). Efficiently mitigating transient execution attacks using the unmapped speculation contract. In 14th USENIX Symposium on Operating Systems Design and Implementation (OSDI 20) (pp. 1139-1154).}
