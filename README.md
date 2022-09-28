# TPEWhy是干什么的
ThreadPoolExecutor(TPE)是Java线程池的核心类，这里通过问问题和回答的形式，来加深对Java线程池理解。  
注意，不是八股文！不是八股文！不是八股文！  
项目最初萌发于本人在复习Java线程池时做的笔记，后为了梳理思路也为了集思广益，整理成项目，方便大家一起学习交流。
# TPEWhy和八股文及面试宝典的区别是什么  
一言以蔽之：对着源码，说自己的理解
既不是八股文式地夸夸其谈，只talk无code，也不是纯geek式扔下带注释的源码让自己看，而是让源码成为回答问题的论据和支撑，目的是彻底明白Why，理顺大方向逻辑，既学习了原理，也能回答问题。
# TPEWhy的问题列表
TPEWhy以问题为引子，为了回答问题翻源码找资料，给出理解和答案。
以下是问题列表，每一个问题都链接到一个专题详细回答。
---
## 1.为什么不建议使用Executors创建线程池
---
## 2.线程池参数理解
---
### 2.1四种经典线程池，都是什么参数？
### 2.2主要使用了哪几种BlockingQueue？
### 2.3使用了无界队列，corePoolSize，maximumPoolSize还有用吗？
### 2.4corePoolSize，maximumPoolSize和BlockingQueue有什么关系？
### 2.5keepAliveTime就是线程最大存活时间吗？
### 2.6四种拒绝策略具体作用？
---
## 3.线程池运行的理解
### 3.1提交一个新task时，流程是怎样的？ 
### 3.2线程池是怎么实现线程“一直运行”的？
### 3.3任务执行过程中出现异常了会怎么样？
### 3.4.shutdown相关
#### 3.4.1shutdown方法执行后，会有什么影响？
原有的queue中任务如何？线程池的线程会如何？如果有新来的task会如何？
### 3.5shutdownnow相关
#### 3.5.1shutdownnow方法执行后，会有什么影响？
原有的queue中任务如何？线程池的线程会如何？如果有新来的task会如何？
#### 3.5.2.drainQueue如何保证一致性？
### 3.6既然interrupt不能暂停线程，那shutdown和shutdownnow为什么还要interrupt？
### 3.7shutdown和shutdownnow的interrupt策略有何区别，对queue中task，新来的task处理原则有何区别？
## 3.8shutdown和shutdownnow一定会触发线程回收吗？
## 3.9什么情况下会触发线程的回收？
---
## 4.什么要使用mainLock？
---
## 5.tryTerminate在干嘛？
---
## 6.为什么总要使用final来存锁？
---

# 其他
项目萌发于复习笔记，非常口语化和简陋，肯定有很多错误和疏漏之处，欢迎大家批评指正，一起批判它，一起丰富它  
想要补充完善contribute的同学可以直接提pr  
有疑问直接到TPEWhy的[Discussion](https://github.com/CaptineNemo/TPEWhy/discussions)区参与讨论（如果没有可以自己创建），或者加微信群交流（纯交流，广告和卖课请勿进谢谢）：  

![31a4e32b033cd192e0bdfdad0999f67](https://user-images.githubusercontent.com/49831244/192768463-dce459b2-e142-4257-a1ad-79fb4e5d0c42.jpg)


