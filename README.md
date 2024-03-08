# GeminiChatbot
 Gemini API Trial 

In Terminal -> 


Last login: Sat Mar  9 04:41:29 on ttys000
pragyan@Pragyans-MacBook-Air ~ % cd Desktop
pragyan@Pragyans-MacBook-Air Desktop % cd cb
pragyan@Pragyans-MacBook-Air cb % python -m venv myenvc 
pragyan@Pragyans-MacBook-Air cb % source myenv/bin/activate 
(myenv) pragyan@Pragyans-MacBook-Air cb % pip install google-generativeai
Requirement already satisfied: google-generativeai in ./myenv/lib/python3.9/site-packages (0.4.0)
Requirement already satisfied: google-auth>=2.15.0 in ./myenv/lib/python3.9/site-packages (from google-generativeai) (2.28.1)
Requirement already satisfied: typing-extensions in ./myenv/lib/python3.9/site-packages (from google-generativeai) (4.10.0)
Requirement already satisfied: protobuf in ./myenv/lib/python3.9/site-packages (from google-generativeai) (4.25.3)
Requirement already satisfied: pydantic in ./myenv/lib/python3.9/site-packages (from google-generativeai) (2.6.3)
Requirement already satisfied: google-ai-generativelanguage==0.4.0 in ./myenv/lib/python3.9/site-packages (from google-generativeai) (0.4.0)
Requirement already satisfied: tqdm in ./myenv/lib/python3.9/site-packages (from google-generativeai) (4.66.2)
Requirement already satisfied: google-api-core in ./myenv/lib/python3.9/site-packages (from google-generativeai) (2.17.1)
Requirement already satisfied: proto-plus<2.0.0dev,>=1.22.3 in ./myenv/lib/python3.9/site-packages (from google-ai-generativelanguage==0.4.0->google-generativeai) (1.23.0)
Requirement already satisfied: googleapis-common-protos<2.0.dev0,>=1.56.2 in ./myenv/lib/python3.9/site-packages (from google-api-core->google-generativeai) (1.62.0)
Requirement already satisfied: requests<3.0.0.dev0,>=2.18.0 in ./myenv/lib/python3.9/site-packages (from google-api-core->google-generativeai) (2.31.0)
Requirement already satisfied: grpcio<2.0dev,>=1.33.2 in ./myenv/lib/python3.9/site-packages (from google-api-core->google-generativeai) (1.62.0)
Requirement already satisfied: grpcio-status<2.0.dev0,>=1.33.2 in ./myenv/lib/python3.9/site-packages (from google-api-core->google-generativeai) (1.62.0)
Requirement already satisfied: cachetools<6.0,>=2.0.0 in ./myenv/lib/python3.9/site-packages (from google-auth>=2.15.0->google-generativeai) (5.3.3)
Requirement already satisfied: rsa<5,>=3.1.4 in ./myenv/lib/python3.9/site-packages (from google-auth>=2.15.0->google-generativeai) (4.9)
Requirement already satisfied: pyasn1-modules>=0.2.1 in ./myenv/lib/python3.9/site-packages (from google-auth>=2.15.0->google-generativeai) (0.3.0)
Requirement already satisfied: pyasn1<0.6.0,>=0.4.6 in ./myenv/lib/python3.9/site-packages (from pyasn1-modules>=0.2.1->google-auth>=2.15.0->google-generativeai) (0.5.1)
Requirement already satisfied: urllib3<3,>=1.21.1 in ./myenv/lib/python3.9/site-packages (from requests<3.0.0.dev0,>=2.18.0->google-api-core->google-generativeai) (2.2.1)
Requirement already satisfied: certifi>=2017.4.17 in ./myenv/lib/python3.9/site-packages (from requests<3.0.0.dev0,>=2.18.0->google-api-core->google-generativeai) (2024.2.2)
Requirement already satisfied: charset-normalizer<4,>=2 in ./myenv/lib/python3.9/site-packages (from requests<3.0.0.dev0,>=2.18.0->google-api-core->google-generativeai) (3.3.2)
Requirement already satisfied: idna<4,>=2.5 in ./myenv/lib/python3.9/site-packages (from requests<3.0.0.dev0,>=2.18.0->google-api-core->google-generativeai) (3.6)
Requirement already satisfied: pydantic-core==2.16.3 in ./myenv/lib/python3.9/site-packages (from pydantic->google-generativeai) (2.16.3)
Requirement already satisfied: annotated-types>=0.4.0 in ./myenv/lib/python3.9/site-packages (from pydantic->google-generativeai) (0.6.0)
WARNING: You are using pip version 21.2.4; however, version 24.0 is available.
You should consider upgrading via the '/Users/pragyan/Desktop/cb/myenv/bin/python3 -m pip install --upgrade pip' command.
(myenv) pragyan@Pragyans-MacBook-Air cb % pip install python-dotenv streamlit
Requirement already satisfied: python-dotenv in ./myenv/lib/python3.9/site-packages (1.0.1)
Requirement already satisfied: streamlit in ./myenv/lib/python3.9/site-packages (1.31.1)
Requirement already satisfied: tornado<7,>=6.0.3 in ./myenv/lib/python3.9/site-packages (from streamlit) (6.4)
Requirement already satisfied: python-dateutil<3,>=2.7.3 in ./myenv/lib/python3.9/site-packages (from streamlit) (2.9.0.post0)
Requirement already satisfied: packaging<24,>=16.8 in ./myenv/lib/python3.9/site-packages (from streamlit) (23.2)
Requirement already satisfied: pyarrow>=7.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (15.0.0)
Requirement already satisfied: requests<3,>=2.27 in ./myenv/lib/python3.9/site-packages (from streamlit) (2.31.0)
Requirement already satisfied: tzlocal<6,>=1.1 in ./myenv/lib/python3.9/site-packages (from streamlit) (5.2)
Requirement already satisfied: click<9,>=7.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (8.1.7)
Requirement already satisfied: pillow<11,>=7.1.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (10.2.0)
Requirement already satisfied: pandas<3,>=1.3.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (2.2.1)
Requirement already satisfied: rich<14,>=10.14.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (13.7.1)
Requirement already satisfied: typing-extensions<5,>=4.3.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (4.10.0)
Requirement already satisfied: cachetools<6,>=4.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (5.3.3)
Requirement already satisfied: gitpython!=3.1.19,<4,>=3.0.7 in ./myenv/lib/python3.9/site-packages (from streamlit) (3.1.42)
Requirement already satisfied: toml<2,>=0.10.1 in ./myenv/lib/python3.9/site-packages (from streamlit) (0.10.2)
Requirement already satisfied: importlib-metadata<8,>=1.4 in ./myenv/lib/python3.9/site-packages (from streamlit) (7.0.1)
Requirement already satisfied: validators<1,>=0.2 in ./myenv/lib/python3.9/site-packages (from streamlit) (0.22.0)
Requirement already satisfied: altair<6,>=4.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (5.2.0)
Requirement already satisfied: protobuf<5,>=3.20 in ./myenv/lib/python3.9/site-packages (from streamlit) (4.25.3)
Requirement already satisfied: tenacity<9,>=8.1.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (8.2.3)
Requirement already satisfied: numpy<2,>=1.19.3 in ./myenv/lib/python3.9/site-packages (from streamlit) (1.26.4)
Requirement already satisfied: pydeck<1,>=0.8.0b4 in ./myenv/lib/python3.9/site-packages (from streamlit) (0.8.1b0)
Requirement already satisfied: blinker<2,>=1.0.0 in ./myenv/lib/python3.9/site-packages (from streamlit) (1.7.0)
Requirement already satisfied: jinja2 in ./myenv/lib/python3.9/site-packages (from altair<6,>=4.0->streamlit) (3.1.3)
Requirement already satisfied: toolz in ./myenv/lib/python3.9/site-packages (from altair<6,>=4.0->streamlit) (0.12.1)
Requirement already satisfied: jsonschema>=3.0 in ./myenv/lib/python3.9/site-packages (from altair<6,>=4.0->streamlit) (4.21.1)
Requirement already satisfied: gitdb<5,>=4.0.1 in ./myenv/lib/python3.9/site-packages (from gitpython!=3.1.19,<4,>=3.0.7->streamlit) (4.0.11)
Requirement already satisfied: smmap<6,>=3.0.1 in ./myenv/lib/python3.9/site-packages (from gitdb<5,>=4.0.1->gitpython!=3.1.19,<4,>=3.0.7->streamlit) (5.0.1)
Requirement already satisfied: zipp>=0.5 in ./myenv/lib/python3.9/site-packages (from importlib-metadata<8,>=1.4->streamlit) (3.17.0)
Requirement already satisfied: rpds-py>=0.7.1 in ./myenv/lib/python3.9/site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (0.18.0)
Requirement already satisfied: attrs>=22.2.0 in ./myenv/lib/python3.9/site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (23.2.0)
Requirement already satisfied: referencing>=0.28.4 in ./myenv/lib/python3.9/site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (0.33.0)
Requirement already satisfied: jsonschema-specifications>=2023.03.6 in ./myenv/lib/python3.9/site-packages (from jsonschema>=3.0->altair<6,>=4.0->streamlit) (2023.12.1)
Requirement already satisfied: tzdata>=2022.7 in ./myenv/lib/python3.9/site-packages (from pandas<3,>=1.3.0->streamlit) (2024.1)
Requirement already satisfied: pytz>=2020.1 in ./myenv/lib/python3.9/site-packages (from pandas<3,>=1.3.0->streamlit) (2024.1)
Requirement already satisfied: MarkupSafe>=2.0 in ./myenv/lib/python3.9/site-packages (from jinja2->altair<6,>=4.0->streamlit) (2.1.5)
Requirement already satisfied: six>=1.5 in ./myenv/lib/python3.9/site-packages (from python-dateutil<3,>=2.7.3->streamlit) (1.16.0)
Requirement already satisfied: certifi>=2017.4.17 in ./myenv/lib/python3.9/site-packages (from requests<3,>=2.27->streamlit) (2024.2.2)
Requirement already satisfied: charset-normalizer<4,>=2 in ./myenv/lib/python3.9/site-packages (from requests<3,>=2.27->streamlit) (3.3.2)
Requirement already satisfied: urllib3<3,>=1.21.1 in ./myenv/lib/python3.9/site-packages (from requests<3,>=2.27->streamlit) (2.2.1)
Requirement already satisfied: idna<4,>=2.5 in ./myenv/lib/python3.9/site-packages (from requests<3,>=2.27->streamlit) (3.6)
Requirement already satisfied: markdown-it-py>=2.2.0 in ./myenv/lib/python3.9/site-packages (from rich<14,>=10.14.0->streamlit) (3.0.0)
Requirement already satisfied: pygments<3.0.0,>=2.13.0 in ./myenv/lib/python3.9/site-packages (from rich<14,>=10.14.0->streamlit) (2.17.2)
Requirement already satisfied: mdurl~=0.1 in ./myenv/lib/python3.9/site-packages (from markdown-it-py>=2.2.0->rich<14,>=10.14.0->streamlit) (0.1.2)
WARNING: You are using pip version 21.2.4; however, version 24.0 is available.
You should consider upgrading via the '/Users/pragyan/Desktop/cb/myenv/bin/python3 -m pip install --upgrade pip' command.
(myenv) pragyan@Pragyans-MacBook-Air cb % streamlit run qachat.py 

  You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://192.168.107.47:8501

  For better performance, install the Watchdog module:

  $ xcode-select --install
  $ pip install watchdog
            
/Users/pragyan/Desktop/cb/myenv/lib/python3.9/site-packages/urllib3/__init__.py:35: NotOpenSSLWarning: urllib3 v2 only supports OpenSSL 1.1.1+, currently the 'ssl' module is compiled with 'LibreSSL 2.8.3'. See: https://github.com/urllib3/urllib3/issues/3020
  warnings.warn(


