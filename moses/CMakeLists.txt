
ADD_SUBDIRECTORY (comboreduct)
ADD_SUBDIRECTORY (moses)
ADD_SUBDIRECTORY (feature-selection)

# Currently, the pleasure code does not build, as it uses various
# obsolete combo types and routines and etc.  It needs to be ported
# over to the modern combo interfaces.
#
#ADD_SUBDIRECTORY (pleasure)

IF (HAVE_CYTHON)
	ADD_SUBDIRECTORY (cython)
ENDIF (HAVE_CYTHON)
