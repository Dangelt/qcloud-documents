本文档介绍实例的销毁概述与操作方法。更多到期信息可参考 [到期提醒](/doc/product/213/2181) 。

## 概述
 - **手动销毁方式：**包年包月类型实例仅可在回收站中手动销毁；按量计费类型实例支持手动销毁。
 
 - **自动销毁方式：**包年包月类型实例在回收站中 7 个自然日未恢复会自动销毁；按量计费类型实例余额小于 0 状态持续 24 小时后自动销毁。规定时间内完成 [续费](/doc/product/213/6143) 可继续使用。
 
 - **实例数据：**挂载的本地盘和非弹性云硬盘都将一并销毁，数据丢失，请提前备份。弹性云盘不受影响。
 
 - **计费相关：**实例的状态一旦变为销毁中或已销毁时，就不再产生与该实例相关的费用。
 
 - **弹性 IP ：**被销毁实例的弹性 IP（含辅助网卡上的 IP）会继续保留，闲置 IP 会产生费用。如无需保留，请及时释放。

## 销毁包年包月类型实例
仅能销毁处在 [回收站](/doc/product/213/4931) 中的包年包月类型实例，且仅支持通过控制台操作。
 
 1. 登录 [云主机控制台](https://console.qcloud.com/cvm/)  。
 
 2. 单击左侧导航栏【回收站】-【云服务器回收站】，进入云服务器回收列表。
 
 3. 销毁单个实例：列表中找到需要销毁的实例，单击操作按钮【销毁】。
 
 4. 批量销毁实例：勾选所有需要销毁的实例，单击顶部【批量销毁】。
 
 5. 在弹出框中输入验证码，单击【确定】，完成销毁。

## 销毁按量计费类型实例
按量计费实例销毁后，短时间内控制台仍可见。随后该实例将自动从实例列表中移除，服务彻底中断。
### 使用控制台销毁
 1.  登录 [云主机控制台]( https://console.qcloud.com/cvm/) 。

 2. 销毁单个实例：列表中找到需要销毁的实例，右侧单击【更多】-【云主机状态】-【销毁】。
 
 3. 批量销毁实例：勾选所有需要销毁的实例，在列表顶部，单击【更多操作】下拉框，单击【销毁】。不能销毁的实例会显示原因。

### 使用 API 销毁
请参考 [TerminateInstances 接口](/doc/product/213/9395)。
