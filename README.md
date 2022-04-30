# 字母战争 README
该插件是一个在工作之余和同事伙伴一起放松身心，提升工作效率的娱乐插件

# 安装
在vscode 插件市场搜索alphabe-war点击安装即可

# 启动
安装成功后点击左侧G图标,进入游戏列表界面。该界面有两栏
1. ROOM LIST 为房间界面展示当前局域网中正在等待开始的游戏,鼠标hover到该栏有 + 按钮创建游戏。第一次创建需要先输入玩家名称

2. AI SCRIPT LIST 为操作脚本界面，可以自由编辑脚本控制玩家行为

3. 玩家进入且全部为准备状态，房主点击开始游戏启动

## 操作方式
1. **手动模式**  该模式通过上、下、左、右控制方向，空格控制埋雷;
2. **脚本模式**  通过编写js脚本控制玩家进行游戏。目前提供了当前游戏所有存在对象的当前状态和5种行为操作玩家游戏

## 游戏目标
  两方队伍通过消灭字符怪或者对方获取字符，率先抢到HELLO WORLD 所有字符的一方获胜

## 游戏所有对象 
1. 字符怪 被炸后掉落一个字符,每15秒在地图空白点中随机新增两个
2. 普通怪 每15秒在地图新增1个，碰撞可以杀死玩家，获取字符后可变成字符怪
3. 墙 
    * *普通墙* 可以炸碎
    * *硬墙* 不能炸碎
    * *移动墙* 可以移动，用来格挡怪物或者挡住敌方玩家
    * *时间墙* 倒计时，玩家被怪物碰撞后回到出生点位
4. 道具 
   雷长度增强 获取后爆炸增强
5. 玩家 玩家分为两队，可以通过埋雷消灭字符怪、拾取字符。玩家死亡会掉落一个字符，且回到出生点位，限制5秒后

##  渲染方式
 游戏提供两种展示方式 1 中文模式[默认] 2 ascii模式 
