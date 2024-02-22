# Producing-data-from-the-cantilever-beam
This repository is regarding generating data from the excitation of the cantilever beam.
## How to run:
1. Cantileverbeam_experiment_data_generation.vi:  This is the LabVIEW code for generating data.
1. Input_Signal:  This folder contains the input signal (pre-produced as requirements) as a .txt file. This signal feeds to the shaker as an excitation signal.
2. Save_Data: This folder will save the generated data as a .lvm file. 




## Test Bench and setup explanation 
The experimental setup is shown in Figure 1. For the experiment purpose, a steel cantilever beam structure of 759x 50.66 x 5.14 mm is used and a single Integral Electronics Piezoelectric (IEPE) accelerometer (model J352C33 manufactured by PCB Piezotronics) is mounted close to the edge of the beam structure. This accelerometer has a frequency range of 0.5 Hz to 9k Hz with a sensitivity of 100 mV/g. The sensor data is digitized using a 24-bit NI-9234 IEPE signal conditioner manufactured by National Instruments. The beam is excited by an electromagnetic shaker (model V203R manufactured by LDS), with a useful frequency range of 5-13000Hz and a peak sine force of 17.8N, and is driven by a power amplifier (model PA25E-CE manufactured by LDS). A 45 N load cell (model MLP-10 manufactured by Transducer Techniques) is mounted in-between the shaker and beam structure. A 24-bit bridge input signal conditioner (NI-9237 manufactured by National Instruments) is used to acquire the load-cell data. The experiment is run through a control computer with a Virtual Instrument written in LabVIEW.



![plot](./images/testbench_final.png)

Figure 1: Experimental setup of a cantilever beam with key components and data acquisition setup.







<table class="tg">
<thead>
  <tr>
    <th class="tg-7btt" colspan="2">component&nbsp;&nbsp;&nbsp;list for experiment</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-uzvj" rowspan="4">hardware</td>
    <td class="tg-0pky">Integral Electronics   Piezoelectric (IEPE) accelerometer (model J352C33 manufactured by PCB   Piezotronics)</td>
  </tr>
  <tr>
    <td class="tg-0pky">electromagnetic   shaker (model V203R manufactured by LDS)</td>
  </tr>
  <tr>
    <td class="tg-0pky">power&nbsp;&nbsp;&nbsp;amplifier (model PA25E-CE manufactured by LDS)</td>
  </tr>
  <tr>
    <td class="tg-0pky">45&nbsp;&nbsp;&nbsp;N load cell (model MLP-10 manufactured by Transducer Techniques) </td>
  </tr>
  <tr>
    <td class="tg-7btt">beam&nbsp;&nbsp;&nbsp;dimensions</td>
    <td class="tg-0pky">steel cantilever beam,  759x 50.66 x 5.14 mm </td>
  </tr>
  <tr>
    <td class="tg-uzvj" rowspan="5">DAQ&nbsp;&nbsp;&nbsp;system</td>
    <td class="tg-0pky">NI-9263  4-Channel (voltage output module)</td>
  </tr>
  <tr>
    <td class="tg-0pky">NI-9239&nbsp;&nbsp;&nbsp;4-Channel (voltage input module)</td>
  </tr>
  <tr>
    <td class="tg-0pky">NI-9237&nbsp;&nbsp;&nbsp;4-Channel (loadcell as Bridge Analog Input)</td>
  </tr>
  <tr>
    <td class="tg-0pky">NI-9234&nbsp;&nbsp;&nbsp;4-Channel (vibration Input Module )</td>
  </tr>
  <tr>
    <td class="tg-0pky">cDAQ-9174&nbsp;&nbsp;&nbsp;4-Slot</td>
  </tr>
</tbody>
</table>









## Data sets
* Using this labview code and produced all the data sets are available in the below repository with a more detailed explanation.
*Puja Chowdhury, Austin Downey, Jason D. Bakos and Philip Conrad, “Dataset-4-univariate-signal-with-nonstationarity,”
Apr. 2021. [Online]. Available:https://github.com/PujaChowdhury/Dataset-4-Univariate-signal-with-non-stationarity








