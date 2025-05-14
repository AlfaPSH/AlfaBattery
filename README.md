# AlfaBattery

## Optimization
- Changes governor and CPU frecuencies
- Slows frecuency scaling for battery life
- Disables cpu boost if activated via module or the kernel
- Changes some GPU settings to enhance battery life
- Addsome conservative ZRAM settings to save battery
- Adds some LMKD settings to enhance battery life
- Changes the scheduler

## Frecuencies
- The governor is changed to schedutil
- The min frecuency is set to 300000
- The max frecuency is set to 1600000
### Frecuency scaling
- The max frecuency scaling is 50000
- The min frecuency scaling is 100000

## ZRAM
- Changes zram compression to lz4
- Changes swappiness to 30
- Changes the cache pressure to 150

## Scheduler
- The scheduler is set to cfq, if not existant to  bfq, and if not existant to noop
 
## LMKD
- The minfree parameter of the LMK is set to " 73728,86016,98304,122880,159744,204800 "
