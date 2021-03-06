Linux有问必答：如何创建新的亚马逊AWS访问密钥
================================================================================
> **问题**：我在配置一个需要访问我的亚马逊AWS帐号的应用时被要求提供**AWS访问密钥ID**和**秘密访问密钥**，我怎样创建一个新的AWS访问密钥呢？

亚马逊AWS安全凭证用于验证你以及授权任何第三方应用访问你的AWS帐号，有各种不同的AWS安全凭证可用，如密码、访问密钥、多因素身份验证、X.509证书等。

如果你想要创建新的访问密钥（访问密钥ID和秘密访问密钥），请按一下步骤进行。

首先，登录到[AWS控制台][1]。

从顶部栏选择“安全凭证”菜单（图中红色方框所示）。

![](https://farm4.staticflickr.com/3855/14987093969_b106406596_o.png)

在下一页中，选择“访问密钥（访问密钥ID和秘密访问密钥）”选项（图中红色方框所示）。

![](https://farm6.staticflickr.com/5584/15173842295_6110021f8f_z.jpg)

在下一页中，你将看到一个现存访问密钥ID列表（如果有的话）。注意，你不能恢复现存访问密钥ID的“秘密访问密钥”。出于安全的原因，秘密访问密钥只能在你创建新访问密钥时才可见。

![](https://farm4.staticflickr.com/3897/15150859306_cd25d519be_o.png)

点击“创建新访问密钥”（见图示），将会立即创建一个新的访问密钥ID和密码访问密钥对。

![](https://farm4.staticflickr.com/3919/14987346068_232e8c73cd_z.jpg)

要么下载一个包含有新访问密钥的密钥文件，要么复制并粘贴新访问密钥信息。再次提请牢记，一旦你关闭该窗口，秘密访问密钥将不再可用，除非你下载一个密钥文件。

### 多用户AWS帐号 ###
如果你是作为公司身份创建的帐号，多个雇员共享这一公司帐号，你可能想要使用身份和访问管理（IAM）来创建并管理他们的访问密钥。

IAM是一个web服务，它允许一个公司管理多个用户及其与一个AWS帐号关联的安全凭证。使用IAM，多个用户可以作为不同身份登入单一的AWS帐号，并管理他们的安全凭证而不会相互干预对方的密钥。

要管理IAM用户，点击“安全凭证”页面上的“用户”菜单（见图示）。

![](https://farm6.staticflickr.com/5589/14987486468_a9120b1f8e_z.jpg)

然后，你就可以创建一个新的IAM用户并管理他们的安全凭证，比如访问密钥之类的东西。

--------------------------------------------------------------------------------

via: http://ask.xmodulo.com/create-amazon-aws-access-key.html

译者：[GOLinux](https://github.com/GOLinux)
校对：[wxy](https://github.com/wxy)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创翻译，[Linux中国](http://linux.cn/) 荣誉推出

[1]:http://aws.amazon.com/console/
