# SPDX-License-Identifier: GPL-2.0

obj-$(CONFIG_LICAY_LIB_CRYPTO) += lib_crypto.o

lib_crypto-$(CONFIG_LZ4K_COMPRESS) += lz4k/lz4k_encode.o
lib_crypto-$(CONFIG_LZ4K_DECOMPRESS) += lz4k/lz4k_decode.o

CFLAGS_lz4kd/lz4kd_encode.o += -DLZ4K_DELTA -O3
CFLAGS_lz4kd/lz4kd_encode_delta.o += -DLZ4K_DELTA -O3
CFLAGS_lz4kd/lz4kd_decode.o += -DLZ4K_DELTA -O3
CFLAGS_lz4kd/lz4kd_decode_delta.o += -DLZ4K_DELTA -O3
lib_crypto-$(CONFIG_LZ4KD_COMPRESS) += lz4kd/lz4kd_encode.o lz4kd/lz4kd_encode_delta.o
lib_crypto-$(CONFIG_LZ4KD_DECOMPRESS) += lz4kd/lz4kd_decode.o lz4kd/lz4kd_decode_delta.o
