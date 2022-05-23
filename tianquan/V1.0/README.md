# 项目介绍
一个STM32F103C8T6/STM32F103C6T6的超小型核心板，采用M.2-M接口，能够极大方便项目硬件移植以及简化电路设计。（仅成功使用SW以及STMISP烧录程序，未进行功能验证）

# 项目说明
* 已上传的文件包括核心板原理图、PCB、M.2接口的封装（AD）。  

# 更新记录
2021年11月28日
* 创建开源工程。  

2021年11月29日
* README新增更新记录和核心板电路与PCB设计说明。
* 修正原理图与PCB网络对应错误。
* 将SW下载由额外接口改为M.2接口引出。
* 将PCB中GND网络的PIN脚由全铺铜改为与铺铜“十字花”连接。

2021年12月5日
* 完成拓展板V1.0的设计、打板和测试。
* 核心板更新为V1.1。
* 根据实际使用调整M.2封装模型，新增立式M.2接口封装。
* 完成STMISP下载验证（FLYMCU）。
* 完成拓展板的升级设计，新增SW独立接口、BOOT0/1接口，更改M.2接口为立式封装。

2022年5月23日
* 拓展板走线修复

# 注意事项
* 核心板打板请选择板厚**0.8mm**、绿色，并备注：不做半孔工艺（土豪无所谓）**PS：一般工艺都是焊盘镀锡，插拔次数有限！**
* 核心板PCB设计按照回流焊工艺（实际用热风枪吹），所以没有预留手焊空间。
* 有可能会出现PCB与原理图相差的地方，一切以PCB为准。
* 晶振要注意匹配电容不一定是12PF，购买时注意商家的备注。
* 轻触开关尺寸为**3X4X2.5**（应该没有比这个更小尺寸的得了）。
* 想重画PCB的注意M.2接口附近**2mm**内的TOP和BOTTOM层不做铺铜，防止因有可能的剐蹭造成的短路；接地PIN脚要做十字花连接防止立碑或移位现象。
* 测试过程中发现无法读取芯片信息且核心板严重发热，请检查**STM32芯片**焊接是否正常，用热风枪焊接的芯片建议用电烙铁每边按一下防止虚焊（PS：一定要先焊芯片，不然空间太小，没有操作空间）。

# 项目进度
* 原理设计（√）  
* LAYOUT设计（√）  
* PCB打板及焊接（√）
* 程序烧录验证（√）
* 转接底板设计（√）
* 转接底板PCB打板及焊接（√）
* 全功能及验证

# 核心板硬件功能
* SW下载接口（V1.1及后续版本由M.2接口引出）
* 5V转3V3电源转换
* 串口转USB
* 16MBit SPI FLASH
* 电源、串口通信指示灯
* 复位按键

# 核心板实物图
<img src="https://note.youdao.com/yws/api/personal/file/WEB6fcfa6da02f946403bdc9f698390e793?method=download&shareKey=d339eadb7aa42a86350d6023ac862496" alt="image" style="zoom:50%;" />


<img src="https://note.youdao.com/yws/api/personal/file/WEB2265ab93cd0602ce548b2c318d845cf2?method=download&shareKey=1d5c4b1e348459c6e97eaf658c9e98c2" alt="image" style="zoom:50%;" />

<img src="https://note.youdao.com/yws/api/personal/file/WEBc9c810146f6b315e35930ef394197548?method=download&shareKey=deee4ec76e6c228ba9b45fb6633cb295" alt="image" style="zoom:50%;" />


# 核心板电路及PCB设计
AD工程文件均在附件，请自行下载阅读；所有原理都是开源资料没啥好说的；

<img src="https://note.youdao.com/yws/api/personal/file/WEBcb73ad509fb8a6b54081265dfe2ffcac?method=download&shareKey=f53759979c27f9afeecff06324be0a3a" alt="image" style="zoom:50%;" />

# 附加说明
如有错误之处欢迎指正！