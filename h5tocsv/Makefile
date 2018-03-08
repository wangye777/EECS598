all: hdf5_getters.py msdHDF5toCSV.py
        for OBJ in E F G H I J K L M N ; do \
                scp -r umwangye@flux-login4:/scratch/engin_flux/umwangye/MSD/$$OBJ.tar.gz ./ ; \
                tar -xvf $$OBJ.tar.gz ;\
                rm $$OBJ.tar.gz ;\
                python msdHDF5toCSV.py ;\
                mv SongFeatureCSV.csv SongFeatureCSV-$$OBJ.csv ;\
                cp SongFeatureCSV-$$OBJ.csv /home/umwangye/MSDfeatureCSV/ ;\
                rm -r $$OBJ ;\
        done
