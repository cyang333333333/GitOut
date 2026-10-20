init
hashFile
createBLOB
updateIndex
createTree, createTreeHelper
createTreeFromIndex, createTreeFromIndexHelper, pathSorter

added commit(), creates commit files and saves them in objects, then also updates head
added gitwrapper, it is easy to run git commands now
- things i changed: 
- i added the checks for file not existing or directory to throw exception,
- i made it so it still builds root when index only has one file,
- i saved root tree because it didnt before
- i also returned the real root hash not whole string hash like it did before