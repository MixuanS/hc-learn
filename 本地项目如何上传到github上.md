## 安装github

第一步：你需要在电脑上安装GitHub的客户端
![在这里插入图片描述](https://img-blog.csdnimg.cn/673a43f97eeb4e5688092119310d7b31.png)
双击安装包，点击下一步
![在这里插入图片描述](https://img-blog.csdnimg.cn/e9246a8dd42f48f59d22cbb606df5ecd.png)
选择安装路径点下一步
![在这里插入图片描述](https://img-blog.csdnimg.cn/9dbea09155de404785991734ab3d6d50.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/4e5984b67e1841cfb59eb9be29bb5339.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/d67bb513c18345a280c2c7229a37bc73.png)
编辑器默认就行，获取你用Notepad++，那就需要配置它的环境变量
![在这里插入图片描述](https://img-blog.csdnimg.cn/1e6bfd3baf21411585ca846c5583ff40.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/4216c25b9d974e9e912b1be9eb7a420e.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/f8a1877ac388489da5d29b93c4146989.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/d55328eb778649328a4a400aa52d2839.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/4745e8c44c1a47118ef4fb1c4b308a0e.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/db57e153a7354dcd9c1e5b6389095e88.png)
点击install开始安装
![在这里插入图片描述](https://img-blog.csdnimg.cn/ef06a6f6db294d6b843efadea5eea880.png)
安装结束在桌面点击右键会出现创建仓库的选项
![在这里插入图片描述](https://img-blog.csdnimg.cn/56f6601839ac44c3be5fbab7e4a7f159.png)



## Idea中配置Git

第二步：Idea中配置Git的启动程序，依次点击 File->settings->搜索git
![在这里插入图片描述](https://img-blog.csdnimg.cn/b07c42f56d51465fa23da47a03211b42.png)
设置此页面中的Path to Git executable也就是Git的启动程序，就是Git安装目录下bin中的git.exe，选中后点击右侧的Test
![在这里插入图片描述](https://img-blog.csdnimg.cn/4d67b7f3fc4048c9b186707277925784.png)

------

第三步：Idea连接GitHub并认证，依次点击 File->settings->搜索github

![在这里插入图片描述](https://img-blog.csdnimg.cn/b6e00034fa2c41288c01012be124e52e.png)
在这个页面你需要配置Git的用户名和密码，点击加号
![在这里插入图片描述](https://img-blog.csdnimg.cn/a360095d5e5547c7a943fe521f1d0d6f.png)
对于Idea我建议你选择第二个，因为其他的方式Idea获取不到Token认证，还要手动去github上配置很麻烦
![在这里插入图片描述](https://img-blog.csdnimg.cn/fe71fef4d03744acbfc4c7d68dcdec64.png)
点击Generate，在跳出的浏览器页面中输入你的git账号
![在这里插入图片描述](https://img-blog.csdnimg.cn/4570365a001e4e5ab0e0c637f5f21c4c.png)



## github秘钥生成

登录成功会进入Token令牌的生成界面
![在这里插入图片描述](https://img-blog.csdnimg.cn/01c143cd042a4323906fca96ef525969.png)
令牌名字、有效期、令牌的权限这个你自己根据需要去配置，配置完之后点击最下面的生成Token按钮
![在这里插入图片描述](https://img-blog.csdnimg.cn/9f917e0c41f74f3996a2fff2f6b8bf03.png)
你如果后面想找到你创建的Token，你可以点击你的头像->settings->
![在这里插入图片描述](https://img-blog.csdnimg.cn/52a75e5336bc44599f1c9d3289fb24c3.png)
在左侧配置列表最后一项
![在这里插入图片描述](https://img-blog.csdnimg.cn/cb1457692b904e3cbe5569276ecbcf5f.png)
点击后，在出现下图页面中点击Tokens列表就可以查看并操作这个Token
![在这里插入图片描述](https://img-blog.csdnimg.cn/1ef499d920f040f1b3c60b57001ba208.png)
言归正传，在你创建好Token之后，你会拿到一个秘钥
![在这里插入图片描述](https://img-blog.csdnimg.cn/054f8e81131c4c59aefb74d18376fc16.png)
把这个秘钥复制下来粘贴到Idea中
![在这里插入图片描述](https://img-blog.csdnimg.cn/35afa2ee7fc8492f82406b10e116c33f.png)
然后点击Add
![在这里插入图片描述](https://img-blog.csdnimg.cn/d67ce5eb5c1e4f73916aec6df7848d71.png)
此时你就可以进行你项目的上传了，打开你要上传的项目，在[VCS](https://so.csdn.net/so/search?q=VCS&spm=1001.2101.3001.7020)中点击Create Git Repository，默认在当前项目主路径创建git本地仓库
![在这里插入图片描述](https://img-blog.csdnimg.cn/0d2f2b4d10d74359a49f517dac65a162.png)



## 仓库上传github

随后你的功能栏会多出一个Git选项，选择GitHub中的Share Project on GitHub
![在这里插入图片描述](https://img-blog.csdnimg.cn/21de8e66a50849f8b634a494fa7a5e64.png)
填写git上的仓库name，其他两个按需求写，也可以默认，注意这里的name值只能是一个没有的仓库名，填好之后点击share
![在这里插入图片描述](https://img-blog.csdnimg.cn/d7dd7e1ca60043489e08e5a691e57866.png)
此时远程仓库就好了，当你要提交代码的时候，右键单击项目在git中，先add后commit最后在push即可
![在这里插入图片描述](https://img-blog.csdnimg.cn/43c43c8d36fb4f4181561ddb8df1838d.png)
提交后你就可以在git中看到你的项目和代码了
![在这里插入图片描述](https://img-blog.csdnimg.cn/4888b32d81754f8a8653e4976b378130.png)

------

如果你想要上传到一个已有的仓库里面，就先不要操作`VCS`开始的步骤，而是在idea有了github的用户连接后，去我的电脑中点开项目所在的路径，在路径这种右键后点击`git bash here`，在出来的黑窗口中输入如下命令，注意如下命令中用的是ssh路径，使用前提是你要有SSH认证，如果没有，就改用http路径

```bash
git init
git remote add origin git@github.com:{github用户名}/{repository名}.git
12
```

上面的命令运行后回到idea直接就可操作add-》commit-》Push了，其实主要是为了`git remote`自定义连接远程仓库，其实很多人都选择idea写代码，然后黑窗口git提交这种方式，因为idea很呆板，只使用它，就允许你提交在一个由它新建的仓库中，而且提交的时候必须写描述

------

最后要注意，Token其实不好用，因为除了刚创建的时候你可以看到Token值，那个时候你如果没有保存，那这个Token就相当于废了，所以你可以配置[公钥](https://so.csdn.net/so/search?q=公钥&spm=1001.2101.3001.7020)在管理使用上比Token方便，而且你配置了ssh公钥后你才可以使用ssh的连接推送项目代码

第一步：确保需要公钥的电脑上有Git的SSH信息

右键桌面空白处，选择Git Bash Here打开命令窗口，配置用户名和邮箱（如果已经配置，就跳过）

```bash
git config --global user.name "username"
git config --global user.email "email"
12
```

之后就会在你的用户目录下，比如C:\Users\Administrator下会有一个.gitconfig文件，内容为

```bash
[user]
name = xxx
email = xxx@xxx.com

注1：username和email即github的账户名称和注册邮箱
注2：git config命令的–global参数，用了这个参数，表示你这台机器上所有的Git仓库都会使用这个配置
123456
```

有了用户名和密码，我们查看同目录下是否有`.ssh`这个文件，如果没有，则在Git Bash Here窗口中运行下面的命令生成，邮箱用你github绑定的邮箱

```bash
ssh-keygen -t rsa -C "xxx@xx.com"
1
```

运行后根据提示，点三次回车，期间不要输入任何东西。
![在这里插入图片描述](https://img-blog.csdnimg.cn/e2818da46fd44564ada31b17b8891067.png)
此时我们就可以点击进入`.ssh`目录
![在这里插入图片描述](https://img-blog.csdnimg.cn/3fb803407739454eaaaa66798de96afb.png)

```bash
id_rsa(私钥，不能泄露出去)
id_rsa.pub(公钥)
known_hosts(不管有没有，如果有也不用管)
123
```

第二步：在GitHub上点击Settings，选择里面的SSH and GPG
![在这里插入图片描述](https://img-blog.csdnimg.cn/a0e1277837184813b0df86c3f8f74f35.png)
点开后你可以看到SSH和GPG两种公钥，你任选一种，一般是SSH用的多，点击创建
![在这里插入图片描述](https://img-blog.csdnimg.cn/75a704c887434f519be52f087e5bea69.png)
填写名字和公钥类型，key填的是`.ssh`路径中`id_rsa.pub`文件中的内容
![在这里插入图片描述](https://img-blog.csdnimg.cn/c53393a1e82a4c25aa8ab4be84562954.png)
创建好了之后，你可以看到，公钥上的信息
![在这里插入图片描述](https://img-blog.csdnimg.cn/c6b17cabf3eb4850ae9cc90c8cc93561.png)
配置完成后，你就可以用github仓库的ssh路径推送你的代码，本篇博文中，由于项目之前使用http如今已经推送了，所以可以直接在push中用一个新的推送者，从而用ssh路径推送
![在这里插入图片描述](https://img-blog.csdnimg.cn/6ead7236b81142f1bd08235d3974412b.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/676a80c4cd9a49638fbb5a0937f2ee42.png)
把你仓库的SSH路径复制到URL中
![在这里插入图片描述](https://img-blog.csdnimg.cn/bd2a28abb87c4fde88a29e29896ff93f.png)
之后就可以正常提交了，不过单纯对于idea来说，大家也发现了，它就不需要你手动输入路径，除非是像我前面说的，你想要提交到一个已有的仓库里，或者说你换一个推送者才会用到路径，所以说配置ssh其实对于idea的推送来说用处不大

但注意使用公钥本质上是为了在idea中通过第一种方式去直接添加git用户，以及后期提交使用仓库的SSH路径，而不是说不用用户了，用户还是要有的，它只是你的电脑和Github之间除了Token的第二种认证方式
![在这里插入图片描述](https://img-blog.csdnimg.cn/7fb53ec480ad462bb47978adf9cb39a4.png)