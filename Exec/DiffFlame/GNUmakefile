TOP = ../../..
AMREX_HOME ?= ${TOP}/amrex
IAMR_HOME ?= ${TOP}/IAMR
PELELM_HOME ?= ${TOP}/PeleLM

#
# Build configuration
#

PRECISION       = DOUBLE
DEBUG           = FALSE
DIM             = 3
USE_OMP         = FALSE
USE_MPI         = TRUE
VERBOSE         = TRUE
PROFILE         = FALSE
COMM_PROFILE    = FALSE

# Enable flctin namelist
USE_FLCTS       = TRUE

#USE_PARTICLES   = FALSE

# Enable ht.velocity_plotfile option
#USE_VELOCITY    = FALSE

# Enable time-dependent forcing term
#USE_TDEPFORCING = FALSE

Chemistry_Model = C12LU
fEXE_sources += wang_dodecane_phi_1000.f

Blocs   := .

CEXE_sources +=
FEXE_sources += Prob_$(DIM)d.F Prob_F.F
CEXE_headers += 
FEXE_headers += probdata.H Prob_F.H

include $(PELELM_HOME)/Tools/Make/Make.PeleLM

