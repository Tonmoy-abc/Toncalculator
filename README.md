# Toncalculator
It is a simple calulator for addition, subtraction, multiplication,division, squire, to the power, sqire root, log, factorial, sin, cos, tan, cot, sec, cosec, nCr etc.
There are many mathmatical conversions
```python
def add(x,y):
    #return x additioned by y
    return x+y
```
```python
def sub(x,y):
    #return x subtract by y
    return x-y
```
```python
def mul(x,y):
    #reurn x multiplied by y
    return x*y
```
```python
def dev(x,y):
    #return x divided by y
    return x/y
```
```python
def squire(x):
    #return squire of x
    return x*x
```
```python
def power(x,y):
    #return x to the power y
    return x^y
```
```python
def sqroot(x):
    #return the sqire root of x
    return math.sqrt(x)
```
```python
def log(x,y=None):
    """
    Here x ist number and y is te base.Returns natural
    log if 1 argument is passed and log with
    specified base if 2 arguments are passed

    """
    if y != None:
        return math.log(x,y)
    else:
        return math.log(x)
```
```python
def factorial(x):
    #return facetorial of x
    factorial = 1
    if x >= 1:
        for i in range (1,x+1):
            factorial = factorial * i
    return factorial
```
```python
def sin(x):
    #return sin of x
    return math.sin(x)
```
```python
def cos(x):
    #return cos of x
    return math.cos(x)
```
```python
def tan(x):
    #return tan x
    return math.tan(x)
```
```python
def cot(x):
    #return cot x
    cot = math.tan(x)
    return 1/cot
```
```python
def sec(x):
    #return sec x
    sec = math.cos(x)
    return 1/sec
```
```python
def cosec(x):
    #return cosec x
    cosec = math.sin(x)
    return 1/cosec
```
```python
def nCr(n,r):
    """
    return the combination  is the method of selection of 'r' objects from 
    a set of 'n' objects where the order of selection does not matter
    """
    ncr = factorial(n)/(factorial(r)*factorial(n-r))
    return ncr
```
```python
#### Simple mathmathical conversion ####

## Angle Conversions ##
def degTored(x):
    #return x degree to radin
    red = (x*math.pi/180)
    return red
```
```python
def redTodeg(x):
    #return x radian to degree
    deg = (x*180/math.pi)
    return deg
```
```python
def degTomin(x):
    #return x dgree to minute
    min = x*60
    return min
```
```python
def minTodeg(x):
    #return x minute to degree
    deg = x/60
    return deg
```
```python
def degTosec(x):
    #return x dgree to second 
    sec = x*3600
    return sec
```
```python
def secTodeg(x):
    #return x second to degree
    deg = x/3600
    return deg
```
```python
def minTosec(x):
    #return x minute to second
    sec = x*60
    return sec
```
```python
def secTomin(x):
    #return x second to minute  
    min = x/60
    return min
```
```python
## Length Conversions ##
def inTocm(x):
    #return x inches to centimeters
    return x*2.54
```
```python
def cmToin(x):
    #return x centimeters to inches
    return x/2.54  
```
```python
def ftTom(x):
    #return x feet to meters
    return x*0.3048
```
```python
def mToft(x):
    #return x meters to feet 
    return x/0.3048
```
```python
def ydTom(x):
    #return x yard to meter
    return x*0.9144
```
```python
def mToyd(x):
    #return x meter to yard
    return x/0.9144
```
```python
def mileTokm(x):
    #return x mile to kilometre
    return x/0.621367
```
```python
def kmTomile(x):
    #return x kilometre to mile
    return x*0.621367
```
```python
def n_mileTom(x):
    #return x notical mile to meter
    return x*1852
```
```python
def mTon_mile(x):
    #return x meter to notical mile
    return x/1852
```
```python
def pcTokm(x):
    #return x parsec to kilometre
    return x*3.08567758128E+13
```
```python
def kmTopc(x):
    #return x kilometre to parsec
    return x/3.08567758128E+13
```
```python
## Area Conversions ##
def acreTomsq(x):
    #return x acre to squire meter
    return x/0.000247105
```
```python
def msqToacer(x):
    #return x squire meter to acre 
    return x*0.000247105
```
```python
## Volume Conversions ##  
def galToL(type, x):
    #return x galon to liter you must select type here US or UK
    if type == "US" or "us" or "Us":
        return x*3.785412
    elif type == "Uk" or "UK" or "uk":
        return x*4.54609
    else:
        if type == None or type == "":
            print("[-] Error 404 type is empty")
        else:
            print("[-] Error you are not setected US or UK")
```
```python   
def LTogal(type, x):
    #return x liter to galon you must select type here US or UK
    if type == "US" or "us" or "Us":
        return x/3.785412
    elif type == "Uk" or "UK" or "uk":
        return x/4.54609
    else:
        if type == None or type == "":
            print("[-] Error 404 type is empty")
        else:
            print("[-] Error you are not setected US or UK")
```
```python    
## Mass Conversions ##
def ozTog(x):
    #return x ounces to grams
    return x*28.34952 
```
```python
def gTooz(x):
    #return x grams to ounces   
    return x/28.34952
```
```python
def lbTokg(x):
    #return x pounds to kilograms
    return x*0.45359237 
```
```python
def kgTolb(x):
    #return x kilograms to pounds
    return x/0.45359237 
```
```python
## Velocity Conversions ##
def kmphTomps(x):
    #return x kilometre/hour to meter/second
    m = x*1000
    s = 3600
    return m/s
```
```python
def mpsTokmph(x):
    #return x meter/second to kilometre/hour
    km = x/1000
    h = 1/3600
    return km/h
```
```python
## Pressure Conversions ##

def atmToPa(x):
    #retunrn x atmosphere to pascal
    return x*101325
```
```python
def PaToatm(x):
    #return x pascal to atmosphere
    return x/101325
```
```python
def mmHgToPa(x):
    #return x millimetre of mercury to pascal
    return x*133.322365 
```
```python
def PaTommHg(x):
    #return x pascal to millimetre of mercury
    return x/133.322365 
```python
## Energy Conversions ##
def kgfToJpm(x):
    #return Kilogram-force to Joule/meter 
    return x*9.80665 
```
```python
def JpmTokgf(x):
    #return Joule/meter to Kilogram-force
    return x/9.80665
```
```python
def JTocal(x):
    #return Joule to Calories
    return x*4.184
```
```python
def calToJ(x):
    #return Calories to Joule
    return x/4.184
```
```python
## Power Conversions ##
def hpToKW(x):
    #return Horse Power to kilowatt
    KW = {
        "mechanical": x/745.699872,
        "electrical" : x/746,
        "metric" : x/0.73549875
    }
    return KW
```
```python
def KWTohp(x):
    #return Horse kilowatt to Power 
    hp = {
        "mechanical": x/745.699872,
        "electrical" : x/746,
        "metric" : x/0.73549875
    }
    return hp
```
```python
## Temperature Conversions ##
def FtoC(f):
    #return fahrenheit to celsius
    return ((f-32)*5)/9
```
```python
def CtoF(c):
    #return celsius to fahrenheit
    return ((9*c)/5)+32
    
```
