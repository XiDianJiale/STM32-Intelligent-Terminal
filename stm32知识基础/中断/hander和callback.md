Handler是固定的、底层的中断入口
Callback是用户自定义的、灵活的处理逻辑

示例：
// 标准中断处理函数  
void EXTI0_IRQHandler(void)  
{  
    // 1. 调用HAL库标准中断处理函数  
    HAL_GPIO_EXTI_IRQHandler(GPIO_PIN_0);  
    
    // 可以添加额外的中断处理逻辑  
}  


中断回调示例：
1.GPIO中断回调
2.定时器中断回调
3.串口中断回调
4.ADC中断回调
