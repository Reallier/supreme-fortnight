# image-build

Java 镜像构建：

所有 Java 镜像都使用 glibc 家族的 libc，以减少潜在的问题。
文件 README.md 中提到“为了少整活,所有镜像一律使用 glibc 家族的 libc 以减少问题”，这表明项目在构建 Java 镜像时优先选择 glibc 以确保稳定性和兼容性。
PHP 镜像构建：

PHP73 的扩展支持将在 2021 年 12 月 6 日结束。
所有 PHP73 的构建文件将不再更新。
文件 README.md 中提到“PHP73 的扩展支持将会结束于 2021 年 12 月 6 日 所有 PHP73 构建文件不再更新”，这表明项目已经停止对 PHP73 的支持和更新。
Alpine 镜像的限制：

文件 adopt-deprecation.md 中提到“并且这三个版本均不提供 Alpine 镜像,所以他没有独立的 glibc 支持(原生支持)”，这表明项目中的某些版本不支持 Alpine 镜像，因为 Alpine 使用 musl libc 而不是 glibc。
项目结构：

项目根目录下有多个 Markdown 文件，如 README.md 和 adopt-deprecation.md，这些文件提供了项目的基本信息和一些特定的构建说明。