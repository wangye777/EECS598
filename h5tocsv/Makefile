OBJ = A
all: hdf5_getters.py msdHDF5toCSV.py
	scp -r umwangye@flux-login4:/scratch/engin_flux/umwangye/MSD/$(OBJ).tar.gz ./
	tar -xvf $(OBJ).tar.gz
	python msdHDF5toCSV.py
	mv SongCSV.csv SongCSV-$(OBJ).csv 
	rm $(OBJ).tar.gz
	rm -r $(OBJ)
