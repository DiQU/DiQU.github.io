# File Path and CWD

- file path
- CWD: Current Working Directory

#nodeju

- `__dirname`： 获得当前执行文件所在目录的完整目录名
- `__filename`： 获得当前执行文件的带有完整绝对路径的文件名
- `process.cwd()`：获得当前执行 node 命令时候的文件夹目录名
- literal`./` or `path.resolve('./')`：
  - 不使用`require`时候，`./`与`process.cwd()`一样
  - 使用`require`时候，与`__dirname`一样
