# Authentication <a name="Authentication"></a>

Can you find a way to authenticate as admin?

http://challs.dvc.tf:1337/


# How to solve <a name="How to solve"></a>
1. Mencoba login dengan username dan password acak; `Incorrect username/password!`

2. Mencoba login dengan username: 'admin' dan passsword: 'admin'; `How dare you!`

3. Mencoba login dengan sql injection; username: `'or 1=1 --'` password:  `1`

Ternyata berhasil login dengan menggunakan sql injection 

![](https://github.com/PranandaNurW/writeUp-CTF/blob/main/dvCTF/web/Authentication/admin.png)

lalu view page source dan ketemu flagnya

![](https://github.com/PranandaNurW/writeUp-CTF/blob/main/dvCTF/web/Authentication/inspect.png)


#### dvCTF{!th4t_w4s_34sy!} <a name="flag"></a>
