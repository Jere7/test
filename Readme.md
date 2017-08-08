

# compress

mkdir test

cd test

touch file1;
touch file2;
touch file3;

#los mete todos en un tar

tar -cvzf  test.tar.gz *

#podria especificar 1 x 1

tar -cvzf  test.tar.gz file1 file2 file3

#despues crea y se pasa a otro directorio

mkdir extract-test; cd extract-test

#copia el tar a ese directorio

cp ../test.tar.gz .

#y lo descomprime

tar -xvzf test.tar.gz