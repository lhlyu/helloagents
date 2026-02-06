# helloagents

玩转 HelloAgents

## 本地搭建 HelloAgents 步骤

> 本人都在终端跑，以下教程都是建立在codex cli上完成的

1. 安装 [Codex Cli](https://developers.openai.com/codex/cli/) 工具，**Mac用户** 直接执行 `brew install codex` 安装，安装好后打开终端输入 `codex` 回车，如果正常表示这步完成。
2. 由于国内可能不好订阅 openai 的api服务，可以在 [中转站](https://www.right.codes/register?aff=11f46efb) 进行购买套餐，完全够用，不要觉得要花很多钱，你可以想一下，你开发一个产品10元不到的成本。购买成功后在 **令牌管理** 处生成一个 **令牌** 。
3. 安装 [CC](https://github.com/farion1231/cc-switch/releases/latest) 工具，打开链接滑到最下面，按照系统选择需要安装的软件，如果运行发生警告，请在安全性下允许执行。
4. 打开 **CC工具** ，选择 **Codex** 添加供应商，在 **预设供应商** 里找到 **RightCode** 选中，将界面滑到下方的 **API KEY** 位置填写第二步生成的 **令牌** ， 其他参数可自行调整，也可以用默认的。
5. 随便找个临时目录，执行 `git clone git@github.com:hellowind777/helloagents.git` 将克隆到本地，按照下面的步骤移动文件或目录:
   - 将 `helloagents/Codex CLI/AGENTS.md` 文件拷贝到 `~/.codex` 内，**Mac用户** 直接执行 `cp -f "helloagents/Codex CLI/AGENTS.md" ~/.codex/AGENTS.md`
   - 将 `helloagents/Codex CLI/skills/helloagents` 目录拷贝到 `~/.codex/skills` 内，**Mac用户** 直接执行 `cp -R "helloagents/Codex CLI/skills/helloagents" ~/.codex/skills/helloagents`


验证一下，随便找个临时的目录，比如 `tmp` , 打开终端，进入到 `tmp` 目录内，执行 `codex`，它会给出两个选项，第一个是是否把这个目录的所有权限交给codex，第二个是每次都要申请，建议选一；

执行 `$helloagents ` 回车，有 `【HelloAGENTS】- 技能已激活` 输出表示成功，然后你就可以写需求了。下面有些快捷键需要注意:

- `Shift + Enter` 换行
- `Enter` 发生
- `ctrl + v` 粘贴图片
- `?` 查看一些功能快捷键

