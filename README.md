# Application-of-Accelerator-Exc03
import math 


#n is the factor by which the elementary charge is being multiplied
def get_rigidity(m,E_kin,n):
    c=299792458 #speed of light
    q=n*1.602e-19
    p=math.sqrt(((E_kin/c)**2)+2*E_kin*m)
    rigidity=p/q
    print('magnetic rigidity = {} Tm'.format(rigidity))


get_rigidity(3.953e-25,3.432e-9,28) #uranium
get_rigidity(3.270e-25,1.041e-8,77) #gold
get_rigidity(1.673e-27,1.122e-6,1) #proton
get_rigidity(9.109e-31,1.602e-9,1) #electron
