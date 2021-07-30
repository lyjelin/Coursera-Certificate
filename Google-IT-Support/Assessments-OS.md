# Operating Systems and You: Becoming a Power User

## Week 1

### Basic Commands

1. Using a Linux machine, you have the following directory tree:

```
/
|-- home
|   |-- cindy
|       |-- Pictures
|           |--Alaska
|           |--Canada
|       |-- Movies
|-- var
```

If your current path is /home/cindy/Pictures/Canada, and you want to change to the Alaska directory, which of the following commands can you use? Check all that apply.

- [x] **cd ~/Pictures/Alaska**
- [x] **cd ../Alaska**
- [ ] cd /Pictures/Alaska
- [x] **cd /home/cindy/Pictures/Alaska**

2. In Bash, which of the following commands can you use to view a long list of all files in the /home directory? Check all that apply.
- [ ] list -a /home
- [x] **ls -la /home**
- [x] **ls -l -a /home**
- [ ] ls -la ~

3. In Bash, which of the following commands can you use to remove a directory named: "Miscellaneous Directory?"
- [ ] rm Miscellaneous Directory
- [ ] rm -r Miscellaneous Directory
- [ ] rm Miscellaneous\ Directory
- [x] **rm -r Miscellaneous\ Directory**

### File and Text Manipulation

1. In Bash, which of the following commands can you use to view the contents of a document. Check all that apply. 
- [ ] open
- [x] **cat**
- [x] **less**
- [ ] dog

2. In a Linux machine, you have the following files: 

- apple.txt
- banana.jpg 
- chocolate.txt
- orange.txt

What command can you use to search for the word "fruit" in the text files in the above directory? Check all that apply.
- [x] **grep fruit apple.txt chocolate.txt orange.txt**
- [x] **grep fruit *.txt**
- [ ] find fruit apple.txt chocolate.txt
- [ ] find fruit apple.txt chocolate.txt orange.txt

3. In a Linux machine, you have a file named "types_of_fish.txt" and you want to append the word "trout" to the file contents. Which of the following commands can you use?
- [ ] echo trout < types_of_fish.txt
- [ ] echo trout > types_of_fish.txt
- [x] **echo trout >> types_of_fish.txt**
- [ ] echo trout 2> types_of_fish.txt

4. In a Linux machine, you want to list through a directory called /home/ben/Documents and search for the word "important" in the filenames in that directory. Which of the following commands can you use? 
- [x] **ls /home/ben/Documents | grep important**
- [ ] ls /home/ben/Documents >> grep important
- [ ] ls /home/ben/Documents < grep important
- [ ] ls /home/ben/Documents > grep important













