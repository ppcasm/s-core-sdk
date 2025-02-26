####################################################################################################
#
#	Created by S+core IDE V2.6.1		23:03:36	02/24/25
#
####################################################################################################

OUTDIR	= Debug
APPDIR	= C:\Sunplus\S_CORE~1.1

TOOLDIR	= C:\Sunplus\S_CORE~1.1\gnu\bin
INCLUDES =  -I"C:/Users/ppcasm/Desktop/HyperScan-SPG29x-SDK-main/examples/hyperscan/recovery/flashcfw/"
LIBFOLDER = 

CC	= "$(TOOLDIR)\score-elf-gcc"
CPP	= "$(TOOLDIR)\score-elf-g++"
AS	= "$(TOOLDIR)\score-elf-as"
AR	= "$(TOOLDIR)\score-elf-ar"
LD	= "$(TOOLDIR)\score-elf-ld"
NM	= "$(TOOLDIR)\score-elf-nm"
RM	= "$(TOOLDIR)\rm"

OBJCOPY	= "$(TOOLDIR)\score-elf-objcopy"
OBJDUMP	= "$(TOOLDIR)\score-elf-objdump"
LDSCRIPT	= "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\hyperscan_Prog.ld"

CCDEFFLAG	= -mscore7 -mel -g -Wall -nostartfiles
CCADDFLAG	= -DHYPERSCAN
ASDEFFLAG	= -Wa,-gdwarf-2  -x assembler-with-cpp
ASADDFLAG	= 
LDDEFFLAG	= -T$(LDSCRIPT)   -lm -lc -lgcc
LDADDFLAG	= -Wl,-Map,$@.map
RESDEFFLAG	= -EL -Tresource.ld  -b binary
RMFLAG		= -rf

BINFILE		= "$(OUTDIR)\hyperscan.elf"


RESFILES	=

OBJFILES	=\
	"$(OUTDIR)\hyperscan_startup.o"\
	"$(OUTDIR)\main.o"\
	"$(OUTDIR)\libgloss.o"\
	"$(OUTDIR)\uart.o"\
	"$(OUTDIR)\tv.o"\
	"$(OUTDIR)\norflash.o"\
	"$(OUTDIR)\user_irq.o"\
	"$(OUTDIR)\sys_isr.o"\
	"$(OUTDIR)\sys_irq.o"\
	"$(OUTDIR)\i2c.o"\
	"$(OUTDIR)\hs_controller.o"\
	"$(OUTDIR)\ff.o"\
	"$(OUTDIR)\diskio.o"

"$(OUTDIR)\diskio.o" "$(OUTDIR)\diskio.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\fatfs\diskio.c"
	@echo diskio.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\diskio.d" -MT"$(OUTDIR)\diskio.d" -o "$(OUTDIR)\diskio.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\fatfs\diskio.c" 

"$(OUTDIR)\ff.o" "$(OUTDIR)\ff.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\fatfs\ff.c"
	@echo ff.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\ff.d" -MT"$(OUTDIR)\ff.d" -o "$(OUTDIR)\ff.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\fatfs\ff.c" 

"$(OUTDIR)\hs_controller.o" "$(OUTDIR)\hs_controller.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\hs_controller\hs_controller.c"
	@echo hs_controller.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\hs_controller.d" -MT"$(OUTDIR)\hs_controller.d" -o "$(OUTDIR)\hs_controller.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\hyperscan\hs_controller\hs_controller.c" 

"$(OUTDIR)\i2c.o" "$(OUTDIR)\i2c.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\i2c\i2c.c"
	@echo i2c.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\i2c.d" -MT"$(OUTDIR)\i2c.d" -o "$(OUTDIR)\i2c.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\i2c\i2c.c" 

"$(OUTDIR)\sys_irq.o" "$(OUTDIR)\sys_irq.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\sys_irq.c"
	@echo sys_irq.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\sys_irq.d" -MT"$(OUTDIR)\sys_irq.d" -o "$(OUTDIR)\sys_irq.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\sys_irq.c" 

"$(OUTDIR)\sys_isr.o" "$(OUTDIR)\sys_isr.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\sys_isr.s"
	@echo sys_isr.s
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) $(ASDEFFLAG) $(ASADDFLAG) -MMD -MP -MF"$(OUTDIR)\sys_isr.d" -MT"$(OUTDIR)\sys_isr.d" -o "$(OUTDIR)\sys_isr.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\sys_isr.s" 

"$(OUTDIR)\user_irq.o" "$(OUTDIR)\user_irq.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\user_irq.c"
	@echo user_irq.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\user_irq.d" -MT"$(OUTDIR)\user_irq.d" -o "$(OUTDIR)\user_irq.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\irq\user_irq.c" 

"$(OUTDIR)\norflash.o" "$(OUTDIR)\norflash.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\norflash\norflash.c"
	@echo norflash.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\norflash.d" -MT"$(OUTDIR)\norflash.d" -o "$(OUTDIR)\norflash.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\norflash\norflash.c" 

"$(OUTDIR)\tv.o" "$(OUTDIR)\tv.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\tv\tv.c"
	@echo tv.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\tv.d" -MT"$(OUTDIR)\tv.d" -o "$(OUTDIR)\tv.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\tv\tv.c" 

"$(OUTDIR)\uart.o" "$(OUTDIR)\uart.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\uart\uart.c"
	@echo uart.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\uart.d" -MT"$(OUTDIR)\uart.d" -o "$(OUTDIR)\uart.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\uart\uart.c" 

"$(OUTDIR)\libgloss.o" "$(OUTDIR)\libgloss.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\libgloss.c"
	@echo libgloss.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\libgloss.d" -MT"$(OUTDIR)\libgloss.d" -o "$(OUTDIR)\libgloss.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\libs\libgloss.c" 

"$(OUTDIR)\main.o" "$(OUTDIR)\main.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\main.c"
	@echo main.c
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) -MMD -MP -MF"$(OUTDIR)\main.d" -MT"$(OUTDIR)\main.d" -o "$(OUTDIR)\main.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\main.c" 

"$(OUTDIR)\hyperscan_startup.o" "$(OUTDIR)\hyperscan_startup.d": "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\hyperscan_startup.s"
	@echo hyperscan_startup.s
	@$(CC) -c $(CCDEFFLAG) $(CCADDFLAG) -B $(TOOLDIR) $(INCLUDES) $(ASDEFFLAG) $(ASADDFLAG) -MMD -MP -MF"$(OUTDIR)\hyperscan_startup.d" -MT"$(OUTDIR)\hyperscan_startup.d" -o "$(OUTDIR)\hyperscan_startup.o" "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\hyperscan_startup.s" 


all : "$(OUTDIR)" $(BINFILE)

"$(OUTDIR)" :
	@if not exist "$(OUTDIR)/$(NULL)" mkdir "$(OUTDIR)"

LINKLIB	= 

$(BINFILE) : $(RESFILES) $(OBJFILES) $(LINKLIB) $(LDSCRIPT) "C:\Users\ppcasm\Desktop\HyperScan-SPG29x-SDK-main\examples\hyperscan\recovery\flashcfw\Resource.h"
			@echo linking...
			@$(CC) $(CCDEFFLAG) $(CCADDFLAG) -B$(TOOLDIR) "Obj.lst" -o $(BINFILE) "Lib.lst" $(LIBFOLDER) $(LDDEFFLAG) $(LDADDFLAG)
			@$(OBJCOPY) -O binary $@ $@.bin
			@echo creat .srec for simulator...
			@$(OBJCOPY) -O srec $@  $@.srec
.PHONY: clean
clean :
	@$(RM) $(RMFLAG) ".\fatfs.fms"
DEPFILES	=\
	"$(OUTDIR)\hyperscan_startup.d"\
	"$(OUTDIR)\main.d"\
	"$(OUTDIR)\libgloss.d"\
	"$(OUTDIR)\uart.d"\
	"$(OUTDIR)\tv.d"\
	"$(OUTDIR)\norflash.d"\
	"$(OUTDIR)\user_irq.d"\
	"$(OUTDIR)\sys_isr.d"\
	"$(OUTDIR)\sys_irq.d"\
	"$(OUTDIR)\i2c.d"\
	"$(OUTDIR)\hs_controller.d"\
	"$(OUTDIR)\ff.d"\
	"$(OUTDIR)\diskio.d"

ifneq ($(wildcard $(DEPFILES)),)
include $(DEPFILES)
endif

