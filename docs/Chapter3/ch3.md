# 第3节：EXT3文件系统删除文件

​         在Ubuntu中删除文件也很简单，在删除时文件在block中的内容是没有被清除的，只是把inode标记为可用，这样这个标记为可用的inode就会指向新的文件，而之前的文件在磁盘中存在却无法访问到，只有在有新的文件需要占用block的时候，才会被覆盖。