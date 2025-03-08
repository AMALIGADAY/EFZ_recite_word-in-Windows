# Changelog

所有值得记录的对这个项目的更改将会被记录在这个文件里。

## [未发布]

### Added

- 中途退出时保存当前进度
- `CHANGELOG.md`, `CHANGELOG.pdf`, `README.pdf`
- 词库 `B2U3.txt`,`B2U4.txt`,`B3U1.txt`

### Changed

- 将 `请读我.txt` 修改为 `README.md`，并丰富其内容
- 优化了所有文档的格式
- 得分与用时计算微调。具体的，
  用时计算由原来“开始程序就计算”调整为“看到第一个单词首字母时开始计算”，
  而得分则改为正确率，并会在满分时设为 `101.0000%`，颜色计算也相应优化

### Fixed

- 将整活的输入 `Testify` 退出改为输入 `:wq` 退出
- 满分后自动删除订正文件
- 词库增加词性一栏

## [1.0] - 2025-01-03

### Added

- G1FE 词库
- 防手误机制
- 动态正确率
- 输入 Testify 强制退出（无进度保存）

### Changed

- 从 Linux 移植至 Windows

[未发布]: todo
[1.0]: 404 Lost in Atlantis
