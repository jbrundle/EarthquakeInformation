# EarthquakeInformation
A repo for codes relating to earthquake information entropy
#   SIMSEISTimeSeries.py    -   This code uses a Poisson distribution to generate state variable
    #       timeseries similar to those obtained by the various Nowcasting codes of Rundle et al.  
    #       The idea is to use a Poisson distribution, the common model used for seismicity interval statistics.
    #   
    #   Poisson distribution = 1 - exp(t/tau)
    #
    #   This code was written on a Mac using Macports python, but Anaconda python should work as well.
 #################################################################
    #################################################################
    
    #   PARAMETERS
    
    #   Elementary State Variable:     ESV = 1 - exp(t/Tau) 
    
    #   Three Primary Adjustable Parameters Are:
    #
    #       Tau:                Will be a random variable that determines the
    #                           between "large earthquakes"
    #   
    #       Threshold_SV:       Specifies the value of the state variable 
    #                           at which the "large earthquake" occurs. Can
    #                           be a random variable.
    #   
    #       Residual_SV:        Specifies the value of the state variable
    #                           when recovery begins (i.e., essentially the number
    #                           of aftershocks).  Can be a random variable.
    #
    #   Other Main Parameters:
    #
    #       TW, or forecast_interval:   In basic time units, which we assume
    #                           to be months
    #
    #   Total number of months:     NMonths
    
