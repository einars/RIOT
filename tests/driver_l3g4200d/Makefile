include ../Makefile.tests_common

FEATURES_REQUIRED = periph_i2c periph_gpio

USEMODULE += l3g4200d
USEMODULE += xtimer

# set default device parameters in case they are undefined
TEST_L3G4200D_I2C  ?= I2C_DEV\(0\)
TEST_L3G4200D_ADDR ?= 104
TEST_L3G4200D_INT  ?= GPIO_PIN\(0,0\)
TEST_L3G4200D_DRDY ?= GPIO_PIN\(0,1\)

# export parameters
CFLAGS += -DTEST_L3G4200D_I2C=$(TEST_L3G4200D_I2C)
CFLAGS += -DTEST_L3G4200D_ADDR=$(TEST_L3G4200D_ADDR)
CFLAGS += -DTEST_L3G4200D_INT=$(TEST_L3G4200D_INT)
CFLAGS += -DTEST_L3G4200D_DRDY=$(TEST_L3G4200D_DRDY)

include $(RIOTBASE)/Makefile.include
