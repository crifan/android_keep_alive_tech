# 相关基础知识

TODO：

【整理】安卓系统进程优先级和oom_adj、oom_score_adj

---

## 名词术语

* 名词术语
  * `LMK`=`Low Memory Killer`
  * `FC`=`Force Close`
    * `FC对话框` = `FC dialog`= `FC popup`
  * `ANR`=`Application Not Responding`=`程序无响应`

## 保活相关基础知识

* 保活相关基础知识
  * 进程被杀的场景
    * 正常=自然的情况
      * 被LMK杀死
        * oom_adj
        * oom_score_adj
      * 成为空进程，缓存进程后被杀
    * 用户主动
      * 最近任务 -> 一键清理
      * 最近任务 -> 上滑
      * 使用Setting -> forceStop
      * 第三方应用杀进程（如猎豹，360等）
    * 特殊情况 = （应用出现异常）被系统杀死
      * 出现FC或者ANR
