# Tensorflow常用API介绍 #


## 读取图片或文件介绍 ##

    简单的读取一张图片, 或者一个文本等, 可以使用tf.gfile下的函数, 具体成员函数如下

	tf.gfile.Copy(oldpath, newpath, overwrite=False) # 拷贝文件
	tf.gfile.DeleteRecursively(dirname) # 递归删除目录下所有文件
	tf.gfile.Exists(filename) # 文件是否存在
	tf.gfile.FastGFile(name, mode='r') # 无阻塞读取文件
	tf.gfile.GFile(name, mode='r') # 读取文件
	tf.gfile.Glob(filename) # 列出文件夹下所有文件, 支持pattern
	tf.gfile.IsDirectory(dirname) # 返回dirname是否为一个目录
	tf.gfile.ListDirectory(dirname) # 列出dirname下所有文件
	tf.gfile.MakeDirs(dirname) # 在dirname下创建一个文件夹, 如果父目录不存在, 会自动创建父目录. 如果
	文件夹已经存在, 且文件夹可写, 会返回成功
	tf.gfile.MkDir(dirname) # 在dirname处创建一个文件夹
	tf.gfile.Remove(filename) # 删除filename
	tf.gfile.Rename(oldname, newname, overwrite=False) # 重命名
	tf.gfile.Stat(dirname) # 返回目录的统计数据
	tf.gfile.Walk(top, inOrder=True) # 返回目录的文件树



