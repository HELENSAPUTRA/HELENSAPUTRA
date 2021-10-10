- 👋 Hi, I’m @HELENSAPUTRA
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...



2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Web | Portofolio</title>
</head>
<body>
    <div class="container">
        <div class="sidebar">
            <nav>
                <ul>
                    <li><a href="">About</a></li>
                    <li><a href="">Portofolio</a></li>
                    <li><a href="">Blog</a></li>
                    <li><a href="">Contact</a></li>   
                </ul>
            </nav>
        </div>
        <main class="content">
              <section class="hero">
                  <img src="online.png" alt="">
              <div class="hero-content">
                  <h1>Profesi</h1><br></h2>Junior Content Writer at Dicoding</h2><br><br>   
<p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Dignissimos, aperiam dolore assumenda velit repellendus recusandae magni consectetur mollitia facere incidunt inventore perspiciatis  debitis doloribus ullam minima culpa voluptatem. Repellendus, option.</p>
<a href="" class="action-btn">Profile Saya</a>
              </div>
                </section>
        </div>
        <div class="footer">
            <footer>
            <ul>
                <li><img src="instagram.png" alt=""><p>Instagram</p></a></li>
                <li><img src="facebook.png" alt=""><p>Facebook</p></a></li>
                <li><img src="twitter.png" alt=""><p>Twitter</p></a></li>
                <li><img src="telegram.png" alt=""><p>Telegram</p></a></li>
            </ul>
            </footer>
        </div>
    </div>    
</body>
</html>

Kode Lab: style.css
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
68
69
70
71
72
73
74
75
76
77
78
79
80
81
82
83
84
85
86
87
88
89
90
91
92
93
94
95
96
97
98
99
100
101
102
103
104
105
106
107
108
109
110
111
112
113
114
115
116
117
118
119
120
121
122
123
124
125
126
127
128
129
130
131
132
133
134
135
136
137
138
139
140
141
142
143
144
145
146
147
148
149
150
151
152
153
154
155
156
157
158
159
160
161
162
163
164
165
166
167
* {
      margin: 0;
      padding: 0;
 
  }
 
  body {
      background-color: #eff1f2;
      font-family: sans-serif;
  }
 
.content {
    grid-area: content;
}
.sidebar{
    grid-area: sidebar;
    background: linear-gradient(to right, rgba(200,107,142,1), rgba(218,105,250,1),
     rgba(110,125,253,1)) ;
    justify-content: center;
}
.footer {
    grid-area: footer;
    background: white;
}
.container {
    font-size: 1.5em;
    width: 100%;
    height: 100;
    height: 100vh;
    display: grid;
    grid-template-areas: "sidebar" "content" "footer";
    grid-template-columns: 1fr;
    grid-template-rows: 130px 800px 250px;
 
}
 
.content, .sidebar, .footer{
    padding: 1em;
}
 
nav ul {
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: space-between;
    text-align: center;
}
 
nav li{
    list-style: none;
    padding: 1em 0;
}
 
nav li a {
    color: white;
    font-weight: 700;
    opacity: 0.6;
    text-decoration: none;
    transition: 0.3s;
}
 
nav li a:hover {
    opacity: 1;
}
.hero {
    max-width: 90 px;
    margin: 0 auto;
    text-align: center;
}
 
.hero img {
    width: 200px;
}
 
.hero h1 {
    font-size: 2em;
    font-weight: 300;
    color: #373046;
}
 
.hero p {
    font-weight: 300;
    line-height: 1.3em;
    color: #98aBad;
}
 
.action-btn {
    display: inline-block;
    text-decoration: none;
    color: white;
    font-weight: 700;
    background: #567bfb;
    padding: 0.5em 2em;
    border-radius: 60px;
    margin: 1em 0;
    transition: 0.3s;
}
 
footer ul {
max-width: 640px;
margin: 2em auto;
padding: 0;
text-align: center;
display: flex;
flex-direction: row;
 
}
 
footer ul li {
    list-style: none;
    align-self: flex-end;
}
 
footer ul li a{
    text-decoration: none;
    color: #c1c6ce;
}
 
footer ul li img {
    width: 30%;
}
 
footer p {
    font-size: 0.8em;
}
 
@media (min-width: 1040px){
    .container {
        grid-template-areas:"sidebar content" "sidebar footer" ;
        grid-template-rows: 1fr auto ;
        grid-template-columns: 300px 1f;
    }
 
    nav ul{
        display: flex;
        justify-content: space-between;
        flex-direction: column;
    }
    .sidebar{
        background: linear-gradient( rgba(200,107,142,1), rgba(218,105,250,1),
        rgba(110,125,253,1)) ;
        padding-top: 10em;
    }
    .hero{
        text-align: left;
        margin: 7em 0;
    }
    .hero img {
        width: 200px;
        float: right;
    }
    .hero h1{
        font-size: 3em;
    }
    .hero p{
        width: 60%;
    }
    footer ul {
        max-width: 900px;
        margin: 0 auto;
        padding: 1em 0;
    }
 
    footer ul li a img {
        width: 20%;
    }
}

Maka Outputnya:

