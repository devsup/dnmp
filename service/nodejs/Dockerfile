ARG NODE_VERSION=24.13.1-alpine

FROM node:${NODE_VERSION}

# 开启 corepack 并安装 pnpm
RUN corepack enable && corepack prepare pnpm@latest --activate

# 设置国内镜像源
RUN pnpm config set registry https://registry.npmmirror.com

# 工作目录
WORKDIR /www