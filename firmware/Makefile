# Makefile for MicroGuard BMS Firmware

# TODO: Set target MCU (e.g., STM32F103, STM32L4, etc.)
# MCU = stm32f103c8t6

# TODO: Set toolchain
# CC = arm-none-eabi-gcc

# TODO: TensorFlow Lite Micro integration
# TFLM_DIR = lib/tensorflow-lite-micro
# INCLUDES += -I$(TFLM_DIR)
# AS = arm-none-eabi-as
# LD = arm-none-eabi-ld
# OBJCOPY = arm-none-eabi-objcopy
# SIZE = arm-none-eabi-size

# TODO: Set directories
# SRC_DIR = src
# INC_DIR = inc
# LIB_DIR = lib
# BUILD_DIR = build

# TODO: Set source files
# SRCS = $(wildcard $(SRC_DIR)/*.c)
# SRCS += $(wildcard $(LIB_DIR)/*/*.c)

# TODO: Set include directories
# INCLUDES = -I$(INC_DIR)
# INCLUDES += -I$(LIB_DIR)/CMSIS/Include
# INCLUDES += -I$(LIB_DIR)/Device/Include

# TODO: Set compiler flags
# CFLAGS = -mcpu=cortex-m3 -mthumb
# CFLAGS += -Wall -Wextra -O2
# CFLAGS += -ffunction-sections -fdata-sections
# CFLAGS += $(INCLUDES)

# TODO: Set linker flags
# LDFLAGS = -mcpu=cortex-m3 -mthumb
# LDFLAGS += -T linker_script.ld
# LDFLAGS += -Wl,--gc-sections
# LDFLAGS += -specs=nano.specs

# TODO: Build targets
# all: $(BUILD_DIR)/microguard.elf $(BUILD_DIR)/microguard.hex $(BUILD_DIR)/microguard.bin

# $(BUILD_DIR)/microguard.elf: $(SRCS)
# 	@mkdir -p $(BUILD_DIR)
# 	$(CC) $(CFLAGS) $(LDFLAGS) $^ -o $@
# 	$(SIZE) $@

# $(BUILD_DIR)/%.hex: $(BUILD_DIR)/%.elf
# 	$(OBJCOPY) -O ihex $< $@

# $(BUILD_DIR)/%.bin: $(BUILD_DIR)/%.elf
# 	$(OBJCOPY) -O binary $< $@

# TODO: Flash target
# flash: $(BUILD_DIR)/microguard.bin
# 	st-flash write $< 0x8000000

# TODO: Clean target
# clean:
# 	rm -rf $(BUILD_DIR)

# .PHONY: all clean flash
