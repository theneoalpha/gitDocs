

        Whats actually Git is ?

           (Version control system) Git maintain the history of the project ,in case of open source
           which person do which changesand where in the project



        What is GitHub?
            It is online plateform which allows us to host our git repository 






            <------Commands--------->

    ls
        Ye current folder me kitne files/folders hai vo batata hai.

    mkdir dummy.txt
        mkdir command se new folder/file create kr sakte hai.

    cd dummy
        change directory matlab isase hum us file ke andar ja sakte hai.

    git init

        isase ek empty hidden .git file create hoti hai jo ki sare versions ka 
        details store karti hai.

    ls -a 

        isase humme hidden files bhi dikhti hai (Applicable only for Linux and Mac).
        For windows find its homework?                

    git status

        git status check karne ke liye

    git add .

        staging area (guest ko stage me bulana taki ve photo kich sake) files ko add karne ke liye

    cat gitDocs.txt 

        cat command se us file ke content ko dekh sakte hai


    git commit -m "First Commit"

        photograph liya gya stage me


    git restore --stagged gitDocs.txt 

        agar hum photo nhi lena chahte guest ka to unhe bolte hai ki aap thoda piche wait
        kr lijiye cameramen lens change kr rhe hai


    git log

        iss command se history jaan sakte hai kitni baar commit hue hai is given repository ko      


    rm -rf names.txt

        isase names.txt file delete ho jayegi



    git reset < previous stable wale ka hash code copy> 

        isase hum uss stable wale code me aa jayege


     git stash 

        isase hum viewers ko stage ke piche bhej dete hai that means previous stage vale 
        code ko thode der ke liye hide kr dete hai


     git stash pop 

        isase hum use fir se staging area me le aate hai

    git stash clear

        jo stage ke piche wale code hai unhe clear kr dete dubara se kabhi nhi aaye





        <-------Fork concepts ----------->


        jub hum kisi ke open source repository me contributition karna chahte hai to 
        hum uske repo ko fork karenge taki uska repo hamare github profile me copy ho jayege

        fir hame usme new branch banani hai taki uska branch alag ho aur hamara branch(group of 
        code and hamare commits alag ho)


    git branch <branchName>

eg  git branch vikashfeatures
        isase new branch create ho jata hai par us branch me enter karne ke liye hame chcekout
        karna padhta hai


    git checkout vikashfeature


        now ab koi bhi commit karnege vo features branch me hoga



        issi type se jitne bhi contributers honge ve apane apne github profile me fork karke
        apna apna branch create karte hai



    git merge yashfeatures


        iss command se jo yashfeatures vala branch ke code and commits merge ho jayenge vikashfeatures
        me aur dono branch ab
        ek branch ban jayega




             <-----SSH KEYS setup command-------->

            1- Create SSH key
            if you don't have the ssh-key create it like this:

    ssh-keygen -t rsa -b 4096 -C "youremail@example.com"
            2- Check your SSH key
            For this go to your folder ssh, example:

    cd ~/.ssh
            after that, run this command line : ls

            if you have the files: id_rsa, id_rsa.pub so the all is good

            now you need to copy your id_rsa.pub ! (⚠️ NOT the id_rsa) for this run


            
             
    cat id_rsa.pub
             and copy the result

            3- Github / Gitlab
            Go to your github / gitlab.

            Follow the step by your hosting:

            github: Click on your profile -> Settings -> SSH and GPG Keys -> New SSH key
            gitlab: Click on your profile -> preferences -> SSH keys
            past your id_rsa.pub that you have already copied !



                                      
