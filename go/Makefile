
# Linux用ターゲット環境設定
LINUX_TARGET_ENV=GOOS=linux GOARCH=amd64

# Go buildコマンド
BUILD=go build

# 出力先ディレクトリ
DESTDIR=.

.PHONY: build
# Linux向けバイナリのビルド
build:
	CGO_ENABLED=0 $(LINUX_TARGET_ENV) $(BUILD) -o $(DESTDIR)/isuride -ldflags "-s -w"
