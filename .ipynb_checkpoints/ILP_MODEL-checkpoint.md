min \sum_{i\in ALL}\sum_{j\in ALL}\sum_{a\in A} x_{i,j,a}*distance_{i,j}\ +\ \sum_{i\in C}\sum_{a\in A}w_{i,a}\ +\ \sum_{i\in RBLE}\sum_{a\in A}s_{i,a} \\
{}\qquad1)\qquad \sum_{i\in ALL}\sum_{a\in A} x_{i,j,a} = 1\ ,\qquad j\in C\\
{}\qquad2)\qquad \sum_{i\in ALL}\sum_{a\in A} x_{i,j,a} \leq  1\ ,\qquad j\in FO\\
{}\qquad3)\qquad \sum_{j\in REAL} x_{start,j,a} = 1\ ,\qquad a\in A\\
{}\qquad4)\qquad x_{start,j,a} = 0\ ,\qquad j\in FO,\ a\in A\\
{}\qquad5)\qquad \sum_{i\in RBLE} x_{i,s,a} = 1\ ,\qquad a\in A\\
{}\qquad6)\qquad \sum_{i\in ALL} x_{i,h,a}\ -\ \sum_{j\in ALL} x_{h,j,a} = 0\ ,\qquad h\in ALL,\ a\in A\\
{}\qquad7)\qquad x_{i,i,a} = 0\ ,\qquad i\in ALL,\ a\in A\\
{}\qquad8)\qquad c_{j,a} = service_j*\sum_{i\in ALL}x_{i,j,a} \ ,\qquad i\in C,\ a\in A\\
{}\qquad9)\qquad \sum_{i\in ALL}\sum_{j\in o+FO}c_{j,a}*x_{i,j,a} = service_{o}\ ,\qquad a\in A\\
{}\qquad10)\qquad c_{j,a} \geq  x_{i,j,a}\ ,\qquad i\in ALL,\ j\in RBLE,\ a\in A\\
{}\qquad11)\qquad \sum_{i\in ALL}\sum_{i\in o+FO}x_{i,j,a} \geq 1\ ,\qquad a\in A\\
{}\qquad12)\qquad x_{i,j,a} = 0\ ,\qquad i\in o+FO,\ j\in o+FO,\ a\in A\\
{}\qquad13)\qquad x_{i,o,a} = 0\ ,\qquad i\in C,\ a\in A\\
{}\qquad14)\qquad x_{j,j+clients,a} \leq  \sum_{i\in ALL}x_{i,j,a}\ ,\qquad j\in C,\ a\in A\\
{}\qquad15)\qquad \{x_{i,j,a} = 0\ \ if\ i\neq j-clients\}\ ,\qquad i\in REAL,\ j\in FO,\ a\in A\\
{}\qquad16)\qquad window\_start_{i} * \sum_{h\in ALL}x_{h,i,a} \leq s_{i,a}\ ,\qquad i\in C,\ a\in A\\
{}\qquad17)\qquad window\_end_{i} * \sum_{h\in ALL}x_{h,i,a} \geq s_{i,a}\ ,\qquad i\in C,\ a\in A\\
{}\qquad18)\qquad l_{i,j,a}*(s_{i,a} + c_{i,a} + distance_{i,j} + w_{j,a}) \geq l_{i,j,a}*lunch\_start\ ,\\
{}\qquad\qquad\qquad i\in RBLE,\ j\in RBLE,\ a\in A\\
{}\qquad19)\qquad l_{i,j,a}*(s_{i,a} + c_{i,a} + distance_{i,j} + w_{j,a}) \leq l_{i,j,a}*lunch\_end\ ,\\
{}\qquad\qquad\qquad i\in RBLE,\ j\in RBLE,\ a\in A\\
{}\qquad20)\qquad l_{i,j,a}\leq x_{i,j,a}*lunch\_end\ ,\qquad i\in RBLE,\ j\in RBLE,\ a\in A\\
{}\qquad21)\qquad t_{a} = max(s_{i,a},\ i\in RBLE)\ ,\qquad a\in A\\
{}\qquad22)\qquad work\_end*\sum_{i\in RBLE}\sum_{j\in RBLE}l_{i,j,a} \geq t_{a} - lunch\_start\ ,\qquad a\in A\\
{}\qquad23)\qquad work\_end*\sum_{i\in RBLE}\sum_{j\in RBLE}(1-l_{i,j,a}) \geq lunch\_start-t_{a},\ \ a\in A\\
{}\qquad24)\qquad s_{j,a} = \sum_{i\in RBLE,\ i!=j}x_{i,j,a}*(s_{i,a}+c_{i,a}+\\
{}\qquad\qquad\qquad distance_{i,j}+l_{i,j,a}*lunch\_len) + w_{j,a}\ ,\qquad j\in RBLE,\ a\in A\\
{}\qquad25)\qquad \sum_{i\in RBLE}\sum_{j\in RBLE}x_{i,j,a}*distance_{i,j}\ +\\
{}\qquad\qquad\qquad \sum_{i\in ALL}\sum_{j\in RBLE}x_{i,j,a}*service_{j}\ +\\
{}\qquad\qquad\qquad \sum_{i\in RBLE}w_{i,a}\ +\\
{}\qquad\qquad\qquad \sum_{i\in RBLE}\sum_{j\in RBLE}l_{i,j,a}*lunch\_len\ +\\
{}\qquad\qquad\qquad work\_start \leq work\_end\ ,\qquad a\in A\\
\\
{}\qquad\qquad\qquad x_{i,j,a}\in \{0,1\}\ , i\in ALL,\ j\in ALL,\ a\in A\\
{}\qquad\qquad\qquad y_{i,a}\in \mathbb{N}\ , i\in ALL,\ a\in A\\
{}\qquad\qquad\qquad c_{i,a}\in \mathbb{N}\ , i\in ALL,\ a\in A\\
{}\qquad\qquad\qquad w_{i,a}\in \mathbb{N}\ , i\in ALL,\ a\in A\\
{}\qquad\qquad\qquad l_{i,j,a}\in \{0,1\}\ , i\in ALL,\ j\in ALL,\ a\in A\\
{}\qquad\qquad\qquad t_{a}\in \mathbb{N}\ , a\in A\\
\\
{}\qquad\qquad\qquad start = clients+1\\
{}\qquad\qquad\qquad o = 0\\
{}\qquad\qquad\qquad C = \{1,...,clients\}\\
{}\qquad\qquad\qquad ALL = \{0,...2clients+1\}\\
{}\qquad\qquad\qquad REAL = \{0,...,clients\}\\
{}\qquad\qquad\qquad RBLE = ALL-\{s\}\\
{}\qquad\qquad\qquad FO = \{P+2,...,2clients+1\}