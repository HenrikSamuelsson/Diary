# 2016 January 20  
 
## Testing MDK
Wanted to run some LwIP related test projects that was developed with the Microcontroller Devlopment Kit (MDK). MDK is a software development solution for ARM developed  by a company called Keil.

## STM32F4DIS-BB Software examples
Downloaded a zip-file with software examples for the STM32F4DIS-BB board [STM32F4DIS-BB Software Examples](http://www.emcu.it/STM32F4xx/ProtoBoards/STM32F4DIS-BB%20Software%20Examples.zip). The examples in this file was based around projects built either in MDK or EWARW. I choose to the MDK to test the projects.

## TCP Echo Client  
Tried the to build the TCP Echo Client from the examples. The project was for an earlier version of the MDK. I choose to migrate the project. Got a big number of errors when building the source. Replaced an bunch of variable names in LwIP (u8 to uint8_t, u16 to uint16_t and u32 to uint32_t). I later realized that this was a mistake (should instead have defined these in cc.h). This project is probably beyond rescue now and can be abandoned and removed. The original version can be retrieved from the 

## HTTP Server  
Tried the HTTP Server in MDK. Choose to run it in legacy mode this time. Got a bunch off errors again, could fix some errors by setting the processor by the use of a define. Some other errors was fixed by adding defines for u8, u16 and u32 in the cc.h file. There was however some errors left that I failed to fix. Will have to give it another try or change to EWARM to see if things runs more smoothly. Note that it could be so that this project requires the LCD expansion board and I do not have one of these, will have to buy or see if other examples runs without this extra board.  
