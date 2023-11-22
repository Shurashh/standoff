import requests


def getAccount(id):
    headers = {'Accept': '*/*',
            'Accept-Encoding': 'gzip, deflate, br',
            'Accept-Language': 'ru,en;q=0.9,en-GB;q=0.8,en-US;q=0.7',
            'Connection': 'keep-alive',
            'Content-Type': 'application/json',
            'Host': 'store.standoff2.com',
            'Referer': 'https://store.standoff2.com/',
            'Sec-Fetch-Dest': 'empty',
            'Sec-Fetch-Mode': 'cors',
            'Sec-Fetch-Site': 'same-origin',
            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.75 Safari/537.36 Edg/100.0.1185.36',
            'sec-ch-ua': '" Not A;Brand";v="99", "Chromium";v="100", "Microsoft Edge";v="100"',
            'sec-ch-ua-mobile': '?0',
            'sec-ch-ua-platform': '"Windows"',
    }

    try:
        account = requests.get(f'https://store.standoff2.com/api/v1/accounts/{id}', headers=headers).json()
        return account['name'], account['uid'], account['avatar']
    except Exception:
        return 'Аккаунт не найден!'
