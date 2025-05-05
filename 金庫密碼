from random import randint    #設定隨機
 
lowest = 1
highest = 100                       #在規定範圍時產生密碼
answer = randint(lowest, highest)   #產生隨機一個答案
 

while True:
    guess = input('密碼介於 ' + str(lowest) + '-' + str(highest) + ':\n>>')     #ex:所猜的數字小於答案則 提示為答案位於所猜的數與當時最大的數之間

 
 #檢查輸入的內容是否為數字
    try:
        guess = int(guess)              #把字串轉換成整數
    except ValueError:                  #不符合便要求重新輸入數字
        print('格式錯誤，請輸入數字\n')
        continue

 
 #檢查輸入的數字是否介於規定範圍內
    if guess <= lowest or guess >= highest:                                    #所猜的數不在規地範圍內
        print('請輸入 ' + str(lowest) + '-' + str(highest) + ' 之間的整數\n')
        continue

 
 #判斷有沒有猜中密碼
    if guess == answer:      #答對
        print('答對了！')
        break                #猜對了才跳脫迴圈
    elif guess < answer:
        lowest = guess       #所猜的數小於答案 因此變為最小的數
    else:
        highest = guess      #所猜的數大於答案 因此變為最大的數
