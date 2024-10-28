The way I approached this problem was by essentially using one of the best first words to guess in wordle, which in this case I chose 'salet'. After sending this in as a guess, we skim through the list of possible words, and filter it so it contains the words that
  - have the letters that returned 2
  - contain the letters that returned 1 but are not in the same position
  - do not contain any letters that return 0

After creating this list, it enters into a while loop that continues until it receives a message of type "bye". It then filters through the list everytime, checking if the word has the same letters return 2 in the same position, else it removes it from the list. It then picks a random word from the list and sends it and repeats this process.

Some difficulties I had was in the beginning where I misread the spec and thought I could send an assortment of letters, then I realized it must be a proper word, so I had to change my search method and had to import the .txt list. Other problems I had was further filtering the list in the while loop, where I had issues with break and continue, so I only used one way to filter it.