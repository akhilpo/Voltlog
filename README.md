# Voltlog
Voltage Logger

Simple voltage logger using Arduino. Connect the signal to log to A0 pin of arduino and point the --tty to the arduino's tty. Don't forget to flash the provided voltlog hex file to arduino. For more info, visit http://github.com/akhilpo/Voltlog
Press 'Ctrl-c' to quit.

Prerequisites: [Install with 'pip install ...']
    docopt
    pyserial

Usage:
    voltlog (-h | --help)
    voltlog (-v | --version)
    voltlog [-V] [-f <filename>] [-T <interval>] [-R <resolution>] -t <ttyname>

Options:
    -h --help                            Show this screen
    -v --version                         Show version
    -f <filename>, --file=<filename>     Append data to <filename>
    -t <ttyname>, --tty=<ttyname>        TTY handler. eg: /dev/tty0
    -T <interval>, --time=<interval>     Time interval between readings in seconds. [default: 1]
    -R <resolution>, --res=<resolution>  Resolution of the ADC in Volts.
    -V , --verbose                       Print data on screen
