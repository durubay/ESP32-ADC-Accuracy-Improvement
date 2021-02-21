# ESP32-ADC-Accuracy-Improvement
Extracting the ESP32 ADC reference voltage to improve ADC reading accuracy

The 'esp_adc_cal/include/esp_adc_cal.h' API provides a function to correct for differences
in measured voltages caused by variation of ADC reference voltages (Vref) between chips.

By-design the ADC reference voltage is 1100 mV, however the true reference voltage can
vary from device-to-deice and range from 1000 mV to 1200 mV amongst different ESP32's.

Reading the reference voltage enables a correction to be made which then improves ADC reading accuracy. 
