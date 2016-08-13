
## Little timer task

Based on example designed by [Herbert Jaeger](http://www.pdx.edu/sites/www.pdx.edu.sysc/files/Jaeger_TrainingRNNsTutorial.2005.pdf)
This task has two imput signal, a start signal and a duration signal. The target output is a signal which starts at each start signal peek and builds a rectangular signal with length of duration signal value.

![sample](.sample.png =800x)
<table>
  <tr>
    <td><img src="sample.png" width="800"></td>
  </tr>
</table>



For training its usefull to have minimum two output signal. So in this example we use the target output and the inverse output. Otherwise cross entropy does't work.
