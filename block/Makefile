#
# Makefile for the kernel block layer
#

ccflags-$(CONFIG_HISI_BLK_MQ)	:= -DBLK_MQ_NO_PERCPU_REFCOUNT

obj-$(CONFIG_BLOCK) := bio.o elevator.o blk-core.o blk-tag.o blk-sysfs.o \
			blk-flush.o blk-settings.o blk-ioc.o blk-map.o \
			blk-exec.o blk-merge.o blk-softirq.o blk-timeout.o \
			blk-iopoll.o blk-lib.o blk-mq.o blk-mq-tag.o \
			blk-mq-sysfs.o blk-mq-cpu.o blk-mq-cpumap.o ioctl.o \
			genhd.o scsi_ioctl.o partition-generic.o ioprio.o \
			partitions/
obj-$(CONFIG_HISI_MQ_DEBUG)		+= hisi-blk-mq-debug.o
obj-$(CONFIG_HISI_MQ_DISPATCH_DECISION)	+= hisi-blk-mq-dispatch-strategy.o
obj-$(CONFIG_BOUNCE)	+= bounce.o
obj-$(CONFIG_BLK_DEV_BSG)	+= bsg.o
obj-$(CONFIG_BLK_DEV_BSGLIB)	+= bsg-lib.o
obj-$(CONFIG_BLK_CGROUP)	+= blk-cgroup.o
obj-$(CONFIG_BLK_DEV_THROTTLING)	+= blk-throttle.o
obj-$(CONFIG_IOSCHED_NOOP)	+= noop-iosched.o
obj-$(CONFIG_IOSCHED_DEADLINE)	+= deadline-iosched.o
obj-$(CONFIG_IOSCHED_ROW)	+= row-iosched.o
obj-$(CONFIG_IOSCHED_CFQ)	+= cfq-iosched.o
obj-$(CONFIG_IOSCHED_TEST)	+= test-iosched.o
obj-$(CONFIG_IOSCHED_SIO)	+= sio-iosched.o
obj-$(CONFIG_IOSCHED_FIOPS)	+= fiops-iosched.o
obj-$(CONFIG_IOSCHED_TRIPNDROID)        += tripndroid-iosched.o

obj-$(CONFIG_BLOCK_COMPAT)	+= compat_ioctl.o
obj-$(CONFIG_BLK_CMDLINE_PARSER)	+= cmdline-parser.o
obj-$(CONFIG_BLK_DEV_INTEGRITY) += bio-integrity.o blk-integrity.o t10-pi.o
obj-$(CONFIG_HISI_BLOCK_FREQUENCE_CONTROL) += hisi_freq_ctl.o
obj-$(CONFIG_HISI_PARTITION)	+= kirin_partition.o
obj-$(CONFIG_HW_SYSTEM_WR_PROTECT) += software_system_wp.o
obj-$(CONFIG_BLK_DEV_BSG)	+= hisi_blk_scsi_kern.o
obj-$(CONFIG_WBT)		+= blk-stat.o
