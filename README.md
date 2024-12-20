![Augene_Beauty_logo](https://github.com/user-attachments/assets/9b612810-b6fe-485d-a870-d98ae53c73e9)
The Augene Profile Pipeline is responsible for:



1. Scraping and downloading microbiome profile data from scientific papers
2. Performing batch correction and data processing
3. Generating microbiome profiles from raw reads
4. Generating a diagnosis from the microbiome profile with machine learning (TODO)

[U<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
 <head>
  <meta charset="utf-8"/>
  <link rel="shortcut icon" href="data:image/x-icon;base64,AAABAAMAEBAAAAEAIABoBAAANgAAABgYAAABACAAiAkAAJ4EAAAgIAAAAQAgAKgQAAAmDgAAKAAAABAAAAAgAAAAAQAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP///wCAgIAC////AP///wC0tKJHlZWSqI6OmuRxcXn9koaK9J2Ym8uNm5V73PPoFv///wAAAAAD////AP///wCAgIAC////AP//7xCHh4OodHSi/2xqw/9nZ9H/XVuU/9eFqv/njb7/yYiq/5GAiOifqKJV////AAAAAAL///8A////AO3t2w56eoHPdHLH/3Vz3vx4dtz7dXTb/mVimv/XhKn/8ZPG/fSVx/vvlcT/kG+E/32Himb///8AAAAAA////wB0dHageHbO/3585fl5d9r/dnTX/3V02/5mYpz80X2i/eaIuv/ukcD/wXak/I6Maf+OkXD9iIKjL////wCEhFo+c3Kv/4F+6P18etz/e3nd/3l33P57eeT/aWag/9F5oP/sib3+tmuZ/3uEXf/P1YX7zdKG/3x9dbX///8Ac3J9nYKA4f+CgOb7fnzf/3174P58et//bm2v8Vtgc7SdbIHNqWmM/4aLZP/L0YT/0dWH/tfdiP+go3P6YlyWJ3BvmduGg+n/g4Hk/oF+4/6AfuX/bm2k7pCUUUX///8Ajv/jCVBmXqPBxoH/1NmI/c7Uhf/b4Yn9wMWB/2BdcGBraqX6iYbs/4SB5P+Eguj7hYPm/2Vlcov///8AACRtB////wAAAIAWrLB29uHojv/X3on+3eSK+9PYh/9XWVN7bWum+ouI7/+Gg+f/hoTq+4iF6f9lZXKL////ACQAbQf///8AAABoFoF+Xva0snL/y818/uDmiPvZ34n/WVlTe3Jxm9uMiu//iofr/oiG6f6Jhu3/cnGo7oyQQ0X///8A/znjCXF8dKNotpL/Za2O/WuVe/+FkGv9mJ5w/2pqaGBzc3+djYrr/42K8fuKh+v/i4js/oqH6/93dbfxYmJztGaTec1yxJr/gOGu/4nptf+K6Lf+i+q8/2eXhfqDNG8ngIBKPnt6uP+Rjvf9jInr/4yJ7f+Miu3+jor0/25xoP920pz/gOGw/oHerv+H4rL/kPC9+5Ttvf98ioC1////AP///wB0dHSgioff/5SR+/mOi+7/jYvt/4+L8P5scJ78etKe/YXis/+H47P/kO+8/JLxv/92m4f9nXKNL////wD///8A7e3bDnt7hM+Ihdv/ko/4/JSS+PuUkPb+bnKg/4Lapv+Q7739kfO/+43puf9/qJH/mYeUZv///wAAAAADgICAAv///wD//+8QhoaBqIB/sf+Iht7/jYjw/2tvnf+D3Kf/ieS1/4bIpP+AkYfoqJOfVf///wAAAAAC////AP///wCAgIAC////AP///wCwsJdHlZWQqJORn+RzdHv9hZOK9Jecmcuej5l7/+jzFv///wAAAAAD////AP///wD4PwAA4A8AAMAHAACAAwAAgAEAAAABAAADgQAAA8EAAAPBAAADgQAAAAEAAIABAACAAwAAwAcAAOAPAAD4PwAAKAAAABgAAAAwAAAAAQAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP///wD///8A////AP///wEAAAAB////AP///wi6urdDubmxj6ennsuQkIzvc3Nz/YSIh/WWoZzWrrezoLe6t1X///8T////AP///wCAgIAC////AP///wD///8A////AP///wD///8A////Af///wD///8Ax8fDQJeYkLV4eH39WlmM/19dpP9dX6b/WFRr/611j/+/fJ//om2I/4N3ff+Jko7Ntri2Xv///wD///8AgICAAv///wD///8A////AP///wD///8B////AP///wOfn5t9c3N29GRjn/9oZ8P/c3LU/XVy3P9rbdH/YVt8/9eIrv/5mcz/75bE/t+Mt/67epz/fnN5/4uTkKP///8W////AAAAAAL///8A////AP///wH///8A////A5iYkZJoaH3/bWvB/3h23Px4dt3+dHPX/3Rx1v9sbcv/YFp6/82ApP/rj8D/65DA//KVxv/1mcn83424/5t1iP98gX7A////F////wCAgIAC////AAAAAAL///8AkJCHdWZlf/9zcs7/fHrj/Hh32/92ddn/dXTX/3Zz2P9vcM//YFt7/8t9of/pi73/54u7/+eNvf/vk8P/7ZbE/pxsh/xLVU7/iomJqP///wD///8A////Af///wCfn5Y4ZmV07XZ0zv9+fOX8enjc/3p43P94dtv/dnXZ/3d12f9xcdD/YFp6/8h5nf/mh7r/44e3/+qMvf/ljrv/jV59/3F+V/68wH3/gYNp/4uIlWf///8AAAAAAv///wJ3d22pc3G6/4KA5/t9e9//fHre/3t53f96eNz/eHbZ/3l23P50dNb9Ylx+/ch2m/3jg7b+44W2/+CItv+NXXz/bnpW/8XIgv/Y3Yv8ur57/3Fxbtni4uIa////AHl5XTdoZ4b4f3zb/4F+5P5+fN//fXvf/3x63v96edz/ennf/nt54P9xccb/Xlxy/7Rvj//gf7P/3IKw/olZeP9te1b/xsqD/9DVh//P1IX/09iG/pWYcf9nZ3Nt////AISEb35ycLb/hYPr/YB+4f9/feH/fnzh/3173/99e+L+enjX/2dmmfhlZXiwYGBiknJkaqGVZ37pg11x/3eBXP7GyoP/0NWH/87Uhf/R1ob/2eCK+8HFff9tbXWv////BG9vdb16eMn/hYPq/4F/4/+BfuP/gH7i/4B94v59e93/Y2KO+ISEbX7y8uQT////AP///weAjo5aT1tP5L7Cf//T2Ij+ztOF/9HWhv/S14b/2d+K/s3Sgv+BgnLcg4OSI11deeaBf9r/hYPo/4OB5P+DgeX/gX/i/4OB6v10c77/cXFjmv///wL///8A////AP///wD///8AeHN9apuecP/U2Yf/0teG/tPZhv/V24f/2uCJ/tTahv+KjGj6AABINV9egfuGg+P/hoTp/4WC5v+EgeX/goDk/4WD6/1wbq//WFgAQ////wAzMzMFAAAAAVVVVQP///8AAABjEoiLZ/Df5Y7/2d+J/dfch//W3If/2d+H/9vhif6ZnW3/AAA5P19egvuHheX/iIXq/4eE6P+Gg+f/hILl/4eE7P1xb7D/WFgAQ////wAzMzMFAAAAAVVVVQP///8AAABVEnd1WvDEx37/y9GD/dnfif/g54z/4OeL/97kiv6anWz/AAA1P15eeuaFg93/ioft/4iF6f+Hhen/hoPn/4mG7/14d8L/cXFimv///wP///8A////AP///wD///8AenV3a1dyZf9QY1//bGVW/pORY/+trnD/xch7/tTZhP+Pkmn6AABINXBwdb1/fc7/jYry/4mH6v+Jhur/iIbp/4iG6/6Gg+X/Z2aT+IKEaX7y8uQT////AP///wiXgY9bXndp5HXLnv95z6P+dsif/2Wrjv9RcWv/Z3Rk/nyBYv9xcWbbfHyDI4SEa354d73/kI31/YuI6/+LiOz/iofr/4mG6v+Lh+3+hoPi/21soPhnZ3qwYGBikmNza6JhinXpcsWa/3vdq/6C4a//iOi1/4zpt/+O6Lf/kOu8+3O1l/9jVmKv////BHl5WDdraor4iofn/4+M8v6Miez/i4nt/4uI7P+LiOv/i4jt/ouJ8P9+e83/XGBt/223jv952aj/e9uq/n3aqv+D36//huKy/4rntv+Q7r3/lvTC/nupj/9zYmxt////AP///wJ3d2qpfXvF/5KP9vyNiu7/jYru/4yJ7f+Miu7/i4jr/46L8P6FgN79XmZ5/XTMm/1+3q7+f9ys/4Lgr/+G5LP/iue2/4zot/+V9cL8iNWs/3BxcNni4uIa////AP///wCfn5I4aGd17YeE3v+Ukfj8jovu/46L7/+Oi+//jYru/46M8f+FgNv/XmV3/3jMnf+D4rH/g+Cw/4fks/+K57b/jem4/5TywP6Q57n/bYh5/5KIjWf///8AAAAAAgAAAAL///8AkJCFdWtqhf+IheL/lZL5/JCN8P+PjO//j4zv/5GO8/+Hgt3/X2Z4/33Rof+I5rb/h+Sz/4nmtf+N6rn/lPPB/pHruvxxm4T/h3yDqP///wD///8A////Af///wH///8A////A5aWj5JtbIP/g4DW/5SR9vyVkvj+kY7y/5KP9P+Ig97/X2d4/4DUpf+N6rn/jeq4/5Lwvv+U88D8h9qu/3KVgv+Lgoe/////F////wCAgIAC////AP///wD///8B////AP///wOfn5l9dHR39HVzsf+Fg97/k4/x/ZiW/v+Nh+f/YWl7/4ngrv+W+MX/kuy8/onesP52uZb/dH54/5aOk6P///8W////AAAAAAL///8A////AP///wD///8A////Af///wD///8Ax8fDQJWVjbV5eX79amic/3h2vv93crf/WV9r/3W1kP95vZn/aZ2C/3eCfP+Ui5DNu7i7Xv///wD///8AgICAAv///wD///8A////AP///wD///8A////AP///wEAAAAB////AP///wi6urdDuLitj6WmmcuPj4rvc3Nz/YiEh/Whlp3Wt66zoLq3ulX///8T////AP///wD///8C////AP///wD///8A////AP8B/wD8AH8A+AAfAOAADwDgAAcAwAAHAIAAAwCAAAMAgAABAAB8AQAAfgEAAP4BAAD+AQAAfgEAAHwBAIAAAQCAAAMAgAADAMAABwDgAAcA4AAPAPgAHwD8AH8A/wH/ACgAAAAgAAAAQAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD///8A////AP///wD///8A////AP///wD///8A////AP///wD///8A////KO3t7XXFxcWwqqqq25eXl/RwcHD9mJiY9Kurq9vHx8ew8PDwdf///yj///8A////AP///wD///8A////AP///wD///8A////AP///wD///8AAAAAAP///wD///8A////AP///wD///8A////AP///wD///8A9/f3TLS0tLpvb3H/UVFR/1VVWf9bW27/WVlz/1FRUf96ZG//c2Nr/1lWV/9RUVH/d3V2/7m5ubr5+flM////AP///wD///8A////AP///wD///8A////AP///wAAAAAA////AP///wD///8A////AP///wD///8A/f39HLW1tatbW13/V1de/2FgkP9rabv/cG7S/29u0/9paL7/UVFR/9GIrv/wlcX/75bE/8+Irf+ZcYb/XVhb/2FfYP+8vLyr/v7+HP///wD///8A////AP///wD///8A////AAAAAAD///8A////AP///wD///8A////AOvr60l2dnnpVVVZ/2ZlnP9ycdL/c3LW/3Jx1f9xcNT/cG/T/2ppvv9RUVH/zoSs/+yRwf/uk8L/7pPC/++UxP/pk8D/pXaP/1hVV/9/fn/p7+/vSf///wD///8A////AP///wD///8AAAAAAP///wD///8A////AP///wDg4OBWX19h/11dcv9zccr/d3XZ/3Z02P91c9f/dHLX/3Nx1v9xcNT/a2q//1FRUf/Ngqn/6o6+/+uQwP/tksH/7pPD/++Vxf/xl8b/3I64/3Jiav9lY2T/2dnZVv///wD///8A////AP///wAAAAAA////AP///wD///8A5OTkQ1tbXf9hYIH/eHfY/3l32/94dtr/d3ba/3Z12f90c9f/c3LW/3Nx1f9tbMH/UVFR/8l/pf/mirr/6Iy8/+mOvv/qj7//7JHB/++VxP/xl8b/04qx/1RUUv9ZWVj/6+vrQ////wD///8A////AAAAAAD///8A////APX19Q9mZmjfYF98/3t53P97ed3/enjc/3l32/93dtr/dnXZ/3Z02P91c9f/dXTY/25tw/9RUVH/yHyj/+WIuf/libn/54q7/+mNvf/rj7//7JHB/9WJsf9XVlX/Z2hb/3BxX/9vb23f+fn5D////wD///8AAAAAAP///wD///8AkZCSnFpaZ/97edn/fHre/3t53v97ed3/enjc/3l33P94dtv/dnXZ/3V02P92dNj/cG7D/1FRUf/FeaH/4oW2/+OGt//liLj/54q6/+mOvv/Sha3/V1VV/2doW//FyYL/xcqC/19fWf+fn5+c////AP///wAAAAAA////ANjY2DhRUVL/dXPA/3994f9+fOD/fXvf/3x63v97ed3/enjc/3l32/94dtr/eHba/3d12f9xb8T/UVFR/8J1nf/fgLH/4IOz/+KEtf/liLn/zoCq/1dVVf9naFr/w8eA/83Shf/P1Yb/q652/1JSUf/h4eE4////AAAAAAD///8Afn6ApWNigv+BfuL/gH3h/3584P99e9//fHre/3x63v97ed3/eXjc/3l32/95d9v/d3ba/3Fwxf9RUVH/wXSc/9x9r//fgbL/4YO0/8t9pv9XVVT/Z2ha/8LHgf/N0oX/ztOF/8/Uhv/S14b/c3Vh/42Ni6X///8AAAAAAOfn5xJRUVH/eXbG/4F/4/+AfuL/f33h/3584P99e+D/fHrf/3x63v97ed3/e3ne/3p43f9ycMH/Y2OR/1FRUf+NY3j/w3Sd/9x9rv/IeaL/V1VU/2doWv/DyIH/zNGF/87Thf/Q1Yb/0daG/9TZh/+ytnj/UlJS/+/v7xIAAAAAq6urYF1cav+DgeX/goDk/4F/4/+AfuL/f33h/3994f9+fOD/fXvf/3x63v95d9X/YF99/1FRUb9sbG+AZmVmgG1qa4BRUVG/fWBv/1dVVP9naFr/xMiB/83Shv/O04b/z9WG/9HWhv/S14b/1NqH/9TZhv9fYFn/t7e3YAAAAAB6enyeaGeV/4SC5v+DgeX/goDk/4F+4/+BfuP/f33h/3584P9+fOD/fHrb/1xcbv9sbG6g39/fQP///wD///8A////ANra2kBbWlugVVVT/8LHgf/O04X/ztOF/8/Uhf/Q1Yb/0teG/9PZh//V24f/2N6I/4aIZv+IiIeeAAAAAFpaXMx0crX/hYLm/4SC5v+DgeX/goDk/4KA5P+Bf+P/gH7i/3994f9oZ5v/X19hv/Hx8SD///8A////AP///wD///8A////AOfn5yBcXFq/m55w/9DVhv/R1ob/0teG/9LXhv/T2Yb/1dqH/9jdiP/Z34j/o6Zy/2VlY8wAAAAAUVFR7Hx7zP+GhOj/hYLm/4SB5f+Egub/g4Hl/4KA5P+Bf+P/gX/j/1paZP+xsbFA////AP///wD///8A////AP///wD///8A////AKampkBqa17/0teG/9LXhv/T2Yf/1dqH/9bciP/Y3oj/2N6H/9rgiP+5vXr/UlJS7AAAAABRUVH7gX7W/4eE6P+GhOj/hYPn/4WC5v+EgeX/g4Hl/4OB5f9/fNv/UVFR/9zc3AD///8A////AP///wD///8A////AP///wD///8A0NDQAFRUU//R14b/1dqH/9Xbh//W3If/192H/9jeh//a4Ij/3OKI/8PJfv9RUVH7AAAAAFFRUfuCgNj/iIbq/4eE6P+HhOj/hoPn/4WC5v+Egub/hILm/4B+3f9RUVH/3NzcAP///wD///8A////AP///wD///8A////AP///wDLy8sAUlJR/87ThP/W3Ij/192H/9nfiP/Z34j/2uCI/9vhiP/d44j/xMh+/1FRUfsAAAAAUVFR7H99zv+Jh+v/iIXq/4iF6v+Hhen/hoTo/4aD5/+Fgub/hYLm/1taZP+xsbFA////AP///wD///8A////AP///wD///8A////AJWVlUBSUlH/UlJR/25vXf+Ul2z/ur97/9jeh//c44j/3uWJ/97lif+8wXr/UVFR7AAAAABaWlzMd3W4/4qH6/+Kh+v/iYbq/4iF6f+HhOj/iIXp/4aE6P+GhOj/a2qe/19fYr/x8fEg////AP///wD///8A////AP///wDp6ekgW1xcv2SWe/9nm4D/Wm9k/1daVv9RUVH/VlZT/3p8Yf+ipnH/ys+A/6ircv9lZmPMAAAAAHp6fJ5rapf/i4js/4uJ7f+KiOz/iYbq/4mG6v+Ihur/iIbq/4eE6P+FguP/Xl5w/2xsb6Df399A////AP///wD///8A2traQGVnZqBccGX/d9Sk/3vZqf+B367/g+Gw/33No/9qk33/W2lh/1ZXVP9RUVH/U1NR/3d3dZ4AAAAAq6urYF5ea/+Ni+//jInt/4uI7P+LiOz/iofr/4mG6v+Jhur/iIXp/4iF6f+EguD/ZGSB/1FRUb9ra2+AZWdmgGpubIBRUVG/Xn1u/3TOn/9516f/ftyr/4Herf+G47L/iOa1/4vot/+Q7bz/k+++/4PHo/9SVFP/oaGhYAAAAADn5+cSUVFR/4F/z/+Niu7/jInt/4yJ7f+LiOz/i4nt/4qI7P+LiOz/iofr/4mG6v+Jhur/fnzN/2ZljP9RUVH/YpB5/2++lf921KT/edem/3vZqf+A3q3/hOGw/4bjs/+J5rX/juu6/5Dsu/+U8cD/g8Wi/1JTUv/t7e0SAAAAAP///wB+foClZ2aG/46L8P+Oi/D/jYru/4yJ7f+Mie3/i4js/4uI7P+LiOz/iofr/4qH6/+KiOz/eXjA/1FRUf9zyJz/eden/3zaqf982qn/ftys/4Hfrv+G47L/iOW0/4rntv+N6rn/ku++/5XxwP9le2//iYqKpf///wAAAAAA////ANjY2DhRUVL/gH7L/4+M8P+Oi+//jovv/42K7v+Niu7/jIru/4yK7v+Mie3/jInt/4uI7P96eMD/UVFR/3bLoP972an/ftyr/4Herv+D4K//heOy/4jmtf+L6Lf/juu5/5DtvP+V8cD/gcGf/1NUU//l5eU4////AAAAAAD///8A////AJGRkpxdXGn/jYrp/5CN8f+PjPD/j4zw/46L7/+Oi+//jYru/42K7v+Niu7/jYru/3x5wv9RUVH/ec6i/4Herv+B367/hOGw/4bjsv+I5bT/i+i3/43quf+Q7bz/k+++/4/jtv9bY17/nZ6enP///wD///8AAAAAAP///wD///8A9vb2D2Zmad9mZYL/kI3w/5CN8f+QjfH/j4zw/4+M8P+PjPD/j4zw/46L7/+Oi+//fHrD/1FRUf9/0qb/hOGw/4Xjsv+F47L/iOa1/4vot/+O67r/kO28/5Lvvf+S7b3/ZHht/3N1dN/6+voP////AP///wAAAAAA////AP///wD///8A5OTkQ1xcXv9oZ4j/kI3v/5GN8f+RjfH/kI3x/5CN8f+QjfH/kI3x/5CN8f99e8P/UVFR/3/UqP+I5bT/iOW0/4vot/+L6Lf/juu5/4/su/+S773/kem6/2Z9cf9gYmH/6+vrQ////wD///8A////AAAAAAD///8A////AP///wD///8A4ODgVl9fYf9iYnf/iojh/5KP8/+Sj/P/kY7y/5GO8v+RjvL/kY7y/358xf9RUVH/hdmt/4vot/+O67n/juu5/5Dtu/+Q7bv/ku++/4rXrv9hcGj/aGpp/+np6Vb///8A////AP///wD///8AAAAAAP///wD///8A////AP///wD///8A7OzsSXd3eelWVlr/dXOr/5CO7v+TkPT/k5D0/5KP8/+Sj/P/f33F/1FRUf+I267/kO28/5Dsu/+Q7Lv/ku+9/5Douv9zoon/U1VU/4GDgunx8fFJ////AP///wD///8A////AP///wAAAAAA////AP///wD///8A////AP///wD///8A/f39HLW1tatbW13/WVlg/3Bunv+Gg9T/k4/y/5SR9f+Bfsf/UVFR/4vfsv+S773/kOu7/4TKpf9ul4H/VlpY/19hYP/AwMCr////HP///wD///8A////AP///wD///8A////AAAAAAD///8A////AP///wD///8A////AP///wD///8A////APf390y0tLS6cG9y/1FRUf9WVlr/Y2J2/2Fgdv9RUVH/ZYBx/2N1a/9VV1b/UVFR/3R2df+/v7+6+vr6TP///wD///8A////AP///wD///8A////AP///wD///8AAAAAAP///wD///8A////AP///wD///8A////AP///wD///8A////AP///wD///8o7e3tdcXFxbCqqqrbl5eX9HBwcP2YmJj0q6ur28fHx7Dv7+91////KP///wD///8A////AP///wD///8A////AP///wD///8A////AP///wAAAAAA//Af//+AA//+AAD//AAAf/gAAD/wAAAf4AAAD8AAAAfAAAAHgAAAA4AAAAOAAAADAAfAAQAP4AEAH/ABAB/wAQAf8AEAH/ABAA/gAQAHwAGAAAADgAAAA4AAAAPAAAAHwAAAB+AAAA/wAAAf+AAAP/wAAH/+AAD//4AD///wH/8="/>
  <script id="notfound" type="text/javascript">window.onload=function(){document.body.innerHTML=""}</script>
  <script language="javascript" type="text/javascript">
{//-----------------------------------------------------------------------------
// 
// PURPOSE
// 
// Krona is a flexible tool for exploring the relative proportions of
// hierarchical data, such as metagenomic classifications, using a
// radial, space-filling display. It is implemented using HTML5 and
// JavaScript, allowing charts to be explored locally or served over the
// Internet, requiring only a current version of any major web
// browser. Krona charts can be created using an Excel template or from
// common bioinformatic formats using the provided conversion scripts.
// 
// 
// COPYRIGHT LICENSE
// 
// Copyright (c) 2011, Battelle National Biodefense Institute (BNBI);
// all rights reserved. Authored by: Brian Ondov, Nicholas Bergman, and
// Adam Phillippy
// 
// This Software was prepared for the Department of Homeland Security
// (DHS) by the Battelle National Biodefense Institute, LLC (BNBI) as
// part of contract HSHQDC-07-C-00020 to manage and operate the National
// Biodefense Analysis and Countermeasures Center (NBACC), a Federally
// Funded Research and Development Center.
// 
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
// 
// * Redistributions of source code must retain the above copyright
//   notice, this list of conditions and the following disclaimer.
// 
// * Redistributions in binary form must reproduce the above copyright
//   notice, this list of conditions and the following disclaimer in the
//   documentation and/or other materials provided with the distribution.
// 
// * Neither the name of the Battelle National Biodefense Institute nor
//   the names of its contributors may be used to endorse or promote
//   products derived from this software without specific prior written
//   permission.
// 
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
// 
// 
// TRADEMARK LICENSE
// 
// KRONA(TM) is a trademark of the Department of Homeland Security, and use
// of the trademark is subject to the following conditions:
// 
// * Distribution of the unchanged, official code/software using the
//   KRONA(TM) mark is hereby permitted by the Department of Homeland
//   Security, provided that the software is distributed without charge
//   and modification.
// 
// * Distribution of altered source code/software using the KRONA(TM) mark
//   is not permitted unless written permission has been granted by the
//   Department of Homeland Security.
// 
// 
// FOR MORE INFORMATION VISIT
// 
// https://github.com/marbl/Krona/wiki/
// 
//-----------------------------------------------------------------------------
}


var canvas;
var context;
var svg; // for snapshot mode
var collapse = true;
var collapseCheckBox;
var collapseLast;
var showMagnitude = false;
var compress;
var compressCheckBox;
var maxAbsoluteDepthText;
var maxAbsoluteDepthButtonDecrease;
var maxAbsoluteDepthButtonIncrease;
var fontSize = 11;
var fontSizeText;
var fontSizeButtonDecrease;
var fontSizeButtonIncrease;
var fontSizeLast;
var radiusButtonDecrease;
var radiusButtonIncrease;
var shorten;
var shortenCheckBox;
var maxAbsoluteDepth;
var backButton;
var upButton;
var forwardButton;
var snapshotButton;
var snapshotMode = false;
var details;
var detailsName;
var search;
var searchResults;
var nSearchResults;
var useHueCheckBox;
var useHueDiv;
var showMagnitudeCheckBox;
var datasetDropDown;
var datasetButtonLast;
var datasetButtonPrev;
var datasetButtonNext;
var keyControl;
var showKeys = true;
var linkButton;
var linkText;
var frame;

// Node references. Note that the meanings of 'selected' and 'focused' are
// swapped in the docs.
//
var head; // the root of the entire tree
var selectedNode = 0; // the root of the current view
var focusNode = 0; // a node chosen for more info (single-click)
var highlightedNode = 0; // mouse hover node
var highlightingHidden = false;
var nodes = new Array();
var currentNodeID = 0; // to iterate while loading

var nodeHistory = new Array();
var nodeHistoryPosition = 0;

var dataEnabled = false; // true when supplemental files are present

// store non-Krona GET variables so they can be passed on to links
//
var getVariables = new Array();

// selectedNodeLast is separate from the history, since we need to check
// properties of the last node viewed when browsing through the history
//
var selectedNodeLast = 0;
var zoomOut = false;

// temporary zoom-in while holding the mouse button on a wedge
//
var quickLook = false; // true when in quick look state
var mouseDown = false;
var mouseDownTime; // to detect mouse button hold
var quickLookHoldLength = 200;

var imageWidth;
var imageHeight;
var centerX;
var centerY;
var gRadius;
var updateViewNeeded = false;

// Determines the angle that the pie chart starts at.  90 degrees makes the
// center label consistent with the children.
//
var rotationOffset = Math.PI / 2;

var buffer;
var bufferFactor = .1;

// The maps are the small pie charts showing the current slice being viewed.
//
var mapBuffer = 10;
var mapRadius = 0;
var maxMapRadius = 25;
var mapWidth = 150;
var maxLabelOverhang = Math.PI * 4.18;

// Keys are the labeled boxes for slices in the highest level that are too thin
// to label.
//
var maxKeySizeFactor = 2; // will be multiplied by font size
var keySize;
var keys;
var keyBuffer = 10;
var currentKey;
var keyMinTextLeft;
var keyMinAngle;

var minRingWidthFactor = 5; // will be multiplied by font size
var maxPossibleDepth; // the theoretical max that can be displayed
var maxDisplayDepth; // the actual depth that will be displayed
var headerHeight = 0;//document.getElementById('options').clientHeight;
var historySpacingFactor = 1.6; // will be multiplied by font size
var historyAlphaDelta = .25;

// appearance
//
var lineOpacity = 0.3;
var saturation = 0.5;
var lightnessBase = 0.6;
var lightnessMax = .8;
var thinLineWidth = .3;
var highlightLineWidth = 1.5;
var labelBoxBuffer = 6;
var labelBoxRounding = 15;
var labelWidthFudge = 1.05; // The width of unshortened labels are set slightly
							// longer than the name width so the animation
							// finishes faster.
var fontNormal;
var fontBold;
var fontFamily = 'sans-serif';
//var fontFaceBold = 'bold Arial';
var nodeRadius;
var angleFactor;
var tickLength;
var compressedRadii;

// colors
//
var highlightFill = 'rgba(255, 255, 255, .3)';
var colorUnclassified = 'rgb(220,220,220)';

// label staggering
//
var labelOffsets; // will store the current offset at each depth
//
// This will store pointers to the last node that had a label in each offset (or "track") of a
// each depth.  These will be used to shorten neighboring labels that would overlap.
// The [nLabelNodes] index will store the last node with a radial label.
// labelFirstNodes is the same, but to check for going all the way around and
// overlapping the first labels.
//
var labelLastNodes;
var labelFirstNodes;
//
var nLabelOffsets = 3; // the number of offsets to use

var mouseX = -1;
var mouseY = -1;
var mouseXRel = -1;
var mouseYRel = -1;

// tweening
//
var progress = 0; // for tweening; goes from 0 to 1.
var progressLast = 0;
var tweenFactor = 0; // progress converted by a curve for a smoother effect.
var tweenLength = 850; // in ms
var tweenCurvature = 13;
//
// tweenMax is used to scale the sigmoid function so its range is [0,1] for the
// domain [0,1]
//
var tweenMax = 1 / (1 + Math.exp(-tweenCurvature / 2));
//
var tweenStartTime;

// for framerate debug
//
var tweenFrames = 0;
var fpsDisplay = document.getElementById('frameRate');

// Arrays to translate xml attribute names into displayable attribute names
//
var attributes = new Array();
//
var magnitudeIndex; // the index of attribute arrays used for magnitude
var membersAssignedIndex;
var membersSummaryIndex;

// For defining gradients
//
var hueDisplayName;
var hueStopPositions;
var hueStopHues;
var hueStopText;

// multiple datasets
//
var currentDataset = 0;
var lastDataset = 0;
var datasets = 1;
var datasetNames;
var datasetSelectSize = 30;
var datasetAlpha = new Tween(0, 0);
var datasetWidths = new Array();
var datasetChanged;
var datasetSelectWidth = 50;

window.onload = load;

var image;
var hiddenPattern;
var loadingImage;
var logoImage;

function backingScale()
{
	if ('devicePixelRatio' in window)
	{
		if (window.devicePixelRatio > 1)
		{
			return window.devicePixelRatio;
		}
	}
	
	return 1;
}

function resize()
{
	imageWidth = window.innerWidth;
	imageHeight = window.innerHeight;
	
	if ( ! snapshotMode )
	{
		context.canvas.width = imageWidth * backingScale();
		context.canvas.height = imageHeight * backingScale();
		context.canvas.style.width = imageWidth + "px"
		context.canvas.style.height = imageHeight + "px"
		context.scale(backingScale(), backingScale());
	}
	
	if ( datasetDropDown )
	{
		var ratio = 
			(datasetDropDown.offsetTop + datasetDropDown.clientHeight) * 2 /
			imageHeight;
		
		if ( ratio > 1 )
		{
			ratio = 1;
		}
		
		ratio = Math.sqrt(ratio);
		
		datasetSelectWidth = 
			(datasetDropDown.offsetLeft + datasetDropDown.clientWidth) * ratio;
	}
	var leftMargin = datasets > 1 ? datasetSelectWidth + 30 : 0;
	var minDimension = imageWidth - mapWidth - leftMargin > imageHeight ?
		imageHeight :
		imageWidth - mapWidth - leftMargin;
	
	maxMapRadius = minDimension * .03;
	buffer = minDimension * bufferFactor;
	margin = minDimension * .015;
	centerX = (imageWidth - mapWidth - leftMargin) / 2 + leftMargin;
	centerY = imageHeight / 2;
	gRadius = minDimension / 2 - buffer;
	//context.font = '11px sans-serif';
}

function handleResize()
{
	updateViewNeeded = true;
}

function Attribute()
{
}

function Tween(start, end)
{
	this.start = start;
	this.end = end;
	this.current = this.start;
	
	this.current = function()
	{
		if ( progress == 1 || this.start == this.end )
		{
			return this.end;
		}
		else
		{
			return this.start + tweenFactor * (this.end - this.start);
		}
	};
	
	this.setTarget = function(target)
	{
		this.start = this.current();
		this.end = target;
	}
}

function Node()
{
	this.id = currentNodeID;
	currentNodeID++;
	nodes[this.id] = this;
	
	this.angleStart = new Tween(Math.PI, 0);
	this.angleEnd = new Tween(Math.PI, 0);
	this.radiusInner = new Tween(1, 1);
	this.labelRadius = new Tween(1, 1);
	this.labelWidth = new Tween(0, 0);
	this.scale = new Tween(1, 1); // TEMP
	this.radiusOuter = new Tween(1, 1);
	
	this.r = new Tween(255, 255);
	this.g = new Tween(255, 255);
	this.b = new Tween(255, 255);
	
	this.alphaLabel = new Tween(0, 1);
	this.alphaLine = new Tween(0, 1);
	this.alphaArc = new Tween(0, 0);
	this.alphaWedge = new Tween(0, 1);
	this.alphaOther = new Tween(0, 1);
	this.alphaPattern = new Tween(0, 0);
	this.children = Array();
	this.parent = 0;
	
	this.attributes = new Array(attributes.length);
	
	this.addChild = function(child)
	{
		this.children.push(child);
	};
	
	this.addLabelNode = function(depth, labelOffset)
	{
		if ( labelHeadNodes[depth][labelOffset] == 0 )
		{
			// this will become the head node for this list
			
			labelHeadNodes[depth][labelOffset] = this;
			this.labelPrev = this;
		}
		
		var head = labelHeadNodes[depth][labelOffset];
		
		this.labelNext = head;
		this.labelPrev = head.labelPrev;
		head.labelPrev.labelNext = this;
		head.labelPrev = this;
	}
	
	this.canDisplayDepth = function()
	{
		// whether this node is at a depth that can be displayed, according
		// to the max absolute depth
		
		return this.depth <= maxAbsoluteDepth;
	}
	
	this.canDisplayHistory = function()
	{
		var radiusInner;
		
		if ( compress )
		{
			radiusInner = compressedRadii[0];
		}
		else
		{
			radiusInner = nodeRadius;
		}
		
		return (
			-this.labelRadius.end * gRadius +
			historySpacingFactor * fontSize / 2 <
			radiusInner * gRadius
			);
	}
	
	this.canDisplayLabelCurrent = function()
	{
		return (
			(this.angleEnd.current() - this.angleStart.current()) *
			(this.radiusInner.current() * gRadius + gRadius) >=
			minWidth());
	}
	
	this.checkHighlight = function()
	{
		if ( this.children.length == 0 && this == focusNode )
		{
			//return false;
		}
		
		if ( this.hide )
		{
			return false;
		}
		
		if ( this.radiusInner.end == 1 )
		{
			// compressed to the outside; don't check
			
			return false;
		}
		
		var highlighted = false;
		
		var angleStartCurrent = this.angleStart.current() + rotationOffset;
		var angleEndCurrent = this.angleEnd.current() + rotationOffset;
		var radiusInner = this.radiusInner.current() * gRadius;
		
		for ( var i = 0; i < this.children.length; i++ )
		{
			highlighted = this.children[i].checkHighlight();
			
			if ( highlighted )
			{
				return true;
			}
		}
		
		if ( this.radial )
		{
			var angleText = (angleStartCurrent + angleEndCurrent) / 2;
			var radiusText = (gRadius + radiusInner) / 2;
			
			context.rotate(angleText);
			context.beginPath();
			context.moveTo(radiusText, -fontSize);
			context.lineTo(radiusText, fontSize);
			context.lineTo(radiusText + centerX, fontSize);
			context.lineTo(radiusText + centerX, -fontSize);
			context.closePath();
			context.rotate(-angleText);
			
			if ( context.isPointInPath(mouseXRel, mouseYRel) )
			{
				var label = String(this.getPercentage()) + '%' + '   ' + this.name;
				
				if ( this.searchResultChildren() )
			    {
					label += searchResultString(this.searchResultChildren());
				}
				
				if
				(
					Math.sqrt((mouseXRel) * (mouseXRel) + (mouseYRel) * (mouseYRel)) / backingScale() <
					radiusText + measureText(label)
				)
				{
					highlighted = true;
				}
			}
		}
		else
		{
		    for ( var i = 0; i < this.hiddenLabels.length; i++ )
		    {
		        var hiddenLabel = this.hiddenLabels[i];
		        
				context.rotate(hiddenLabel.angle);
				context.beginPath();
				context.moveTo(gRadius, -fontSize);
				context.lineTo(gRadius, fontSize);
				context.lineTo(gRadius + centerX, fontSize);
				context.lineTo(gRadius + centerX, -fontSize);
				context.closePath();
				context.rotate(-hiddenLabel.angle);
				
				if ( context.isPointInPath(mouseXRel, mouseYRel) )
				{
					var label = String(hiddenLabel.value) + ' more';
					
					if ( hiddenLabel.search )
				    {
						label += searchResultString(hiddenLabel.search);
					}
					
					if
					(
						Math.sqrt((mouseXRel) * (mouseXRel) + (mouseYRel) * (mouseYRel)) / backingScale() <
						gRadius + fontSize + measureText(label)
					)
					{
						highlighted = true;
						break;
					}
				}
			}
		}
		
		if ( ! highlighted && this != selectedNode && ! this.getCollapse() )
		{
			context.beginPath();
			context.arc(0, 0, radiusInner, angleStartCurrent, angleEndCurrent, false);
			context.arc(0, 0, gRadius, angleEndCurrent, angleStartCurrent, true);
			context.closePath();
			
			if ( context.isPointInPath(mouseXRel, mouseYRel) )
			{
				highlighted = true;
			}
			
			if
			(
				! highlighted &&
				(angleEndCurrent - angleStartCurrent) *
				(radiusInner + gRadius) <
				minWidth() &&
				this.getDepth() == selectedNode.getDepth() + 1
			)
			{
				if ( showKeys && this.checkHighlightKey() )
				{
					highlighted = true;
				}
			}
		}
		
		if ( highlighted )
		{
			if ( this != highlightedNode )
			{
			//	document.body.style.cursor='pointer';
			}
			
			highlightedNode = this;
		}
		
		return highlighted;
	}
	
	this.checkHighlightCenter = function()
	{
		if ( ! this.canDisplayHistory() )
		{
			return;
		}
		
		var cx = centerX;
		var cy = centerY - this.labelRadius.end * gRadius;
		//var dim = context.measureText(this.name);
		
		var width = this.nameWidth;
		
		if ( this.searchResultChildren() )
		{
			var results = searchResultString(this.searchResultChildren());
			var dim = context.measureText(results);
			width += dim.width;
		}
		
		if
		(
			mouseX > cx - width / 2 &&
			mouseX < cx + width / 2 &&
			mouseY > cy - historySpacingFactor * fontSize / 2 &&
			mouseY < cy + historySpacingFactor * fontSize / 2
		)
		{
			highlightedNode = this;
			return;
		}
		
		if ( this.getParent() )
		{
			this.getParent().checkHighlightCenter();
		}
	}
	
	this.checkHighlightKey = function()
	{
		var offset = keyOffset();
		
		var xMin = imageWidth - keySize - margin - this.keyNameWidth - keyBuffer;
		var xMax = imageWidth - margin;
		var yMin = offset;
		var yMax = offset + keySize;
		
		currentKey++;
		
		return (
			mouseX > xMin &&
			mouseX < xMax &&
			mouseY > yMin &&
			mouseY < yMax);
	}
	
	this.checkHighlightMap = function()
	{
		if ( this.parent )
		{
			this.parent.checkHighlightMap();
		}
		
		if ( this.getCollapse() || this == focusNode )
		{
			return;
		}
		
		var box = this.getMapPosition();
		
		if
		(
			mouseX > box.x - mapRadius &&
			mouseX < box.x + mapRadius &&
			mouseY > box.y - mapRadius &&
			mouseY < box.y + mapRadius
		)
		{
			highlightedNode = this;
		}
	}
	
/*	this.collapse = function()
	{
		for (var i = 0; i < this.children.length; i++ )
		{
			this.children[i] = this.children[i].collapse();
		}
		
		if
		(
			this.children.length == 1 &&
			this.children[0].magnitude == this.magnitude
		)
		{
			this.children[0].parent = this.parent;
			this.children[0].getDepth() = this.parent.getDepth() + 1;
			return this.children[0];
		}
		else
		{
			return this;
		}
	}
*/	
	this.draw = function(labelMode, selected, searchHighlighted)
	{
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
//		var hidden = false;
		
		if ( selectedNode == this )
		{
			selected = true;
		}
		
		var angleStartCurrent = this.angleStart.current() + rotationOffset;
		var angleEndCurrent = this.angleEnd.current() + rotationOffset;
		var radiusInner = this.radiusInner.current() * gRadius;
		var canDisplayLabelCurrent = this.canDisplayLabelCurrent();
		var hiddenSearchResults = false;
		
/*		if ( ! this.hide )
		{
			for ( var i = 0; i < this.children.length; i++ )
			{
				if ( this.children[i].hide && this.children[i].searchResults )
				{
					hiddenSearchResults = true;
				}
			}
		}
*/		
		var drawChildren =
			( ! this.hide || ! this.hidePrev && progress < 1 ) &&
			( ! this.hideAlone || ! this.hideAlonePrev && progress < 1 );
		
//		if ( this.alphaWedge.current() > 0 || this.alphaLabel.current() > 0 )
		{
			var lastChildAngleEnd = angleStartCurrent;
			
			if ( this.hasChildren() )//canDisplayChildren )
			{
				lastChildAngleEnd =
					this.children[this.children.length - 1].angleEnd.current()
					+ rotationOffset;
			}
			
			if ( labelMode )
			{
				var drawRadial =
				!(
					this.parent &&
					this.parent != selectedNode &&
					angleEndCurrent == this.parent.angleEnd.current() + rotationOffset
				);
				
				//if ( angleStartCurrent != angleEndCurrent )
				{
					this.drawLines(angleStartCurrent, angleEndCurrent, radiusInner, drawRadial, selected);
				}
				
				var alphaOtherCurrent = this.alphaOther.current();
				var childRadiusInner;
				
				if ( this == selectedNode || alphaOtherCurrent )
				{
					childRadiusInner =
						this.children.length ?
							this.children[this.children.length - 1].radiusInner.current() * gRadius
						: radiusInner
				}
				
				if ( this == selectedNode )
				{
					this.drawReferenceRings(childRadiusInner);
				}
				
				if
				(
					selected &&
					! searchHighlighted &&
					this != selectedNode &&
					(
						this.isSearchResult ||
						this.hideAlone && this.searchResultChildren() ||
						false
//						this.hide &&
//						this.containsSearchResult
					)
				)
				{
					context.globalAlpha = this.alphaWedge.current();
					
					drawWedge
					(
						angleStartCurrent,
						angleEndCurrent,
						radiusInner,
						gRadius,
						highlightFill,
						0,
						true
					);
					
					if
					(
						this.keyed &&
						! showKeys &&
						this.searchResults &&
						! searchHighlighted &&
						this != highlightedNode &&
						this != focusNode
					)
					{
						var angle = (angleEndCurrent + angleStartCurrent) / 2;
						this.drawLabel(angle, true, false, true, true);
					}
					
					//this.drawHighlight(false);
					searchHighlighted = true;
				}
				
				if
				(
					this == selectedNode ||
//					true
					//(canDisplayLabelCurrent) &&
					this != highlightedNode &&
					this != focusNode
				)
				{
					if ( this.radial != this.radialPrev && this.alphaLabel.end == 1 )
					{
						context.globalAlpha = tweenFactor;
					}
					else
					{
						context.globalAlpha = this.alphaLabel.current();
					}
					
					this.drawLabel
					(
						(angleStartCurrent + angleEndCurrent) / 2,
						this.hideAlone && this.searchResultChildren() ||
						(this.isSearchResult || hiddenSearchResults) && selected,
						this == selectedNode && ! this.radial,
						selected,
						this.radial
					);
					
					if ( this.radial != this.radialPrev && this.alphaLabel.start == 1 && progress < 1 )
					{
						context.globalAlpha = 1 - tweenFactor;
						
						this.drawLabel
						(
							(angleStartCurrent + angleEndCurrent) / 2,
							(this.isSearchResult || hiddenSearchResults) && selected,
							this == selectedNodeLast && ! this.radialPrev,
							selected,
							this.radialPrev
						);
					}
				}
				
				if
				(
					alphaOtherCurrent &&
					lastChildAngleEnd != null
				)
				{
					if
					(
						(angleEndCurrent - lastChildAngleEnd) *
						(childRadiusInner + gRadius) >=
						minWidth()
					)
					{
						//context.font = fontNormal;
						context.globalAlpha = this.alphaOther.current();
						
						drawTextPolar
						(
							this.getUnclassifiedText(),
							this.getUnclassifiedPercentage(),
							(lastChildAngleEnd + angleEndCurrent) / 2,
							(childRadiusInner + gRadius) / 2,
							true,
							false,
							false,
							0,
							0
						);
					}
				}
				
				if ( this == selectedNode && this.keyUnclassified && showKeys )
				{
					this.drawKey
					(
						(lastChildAngleEnd + angleEndCurrent) / 2,
						false,
						false
					);
				}
			}
			else
			{
				var alphaWedgeCurrent = this.alphaWedge.current();
				
				if ( alphaWedgeCurrent || this.alphaOther.current() )
				{
					var currentR = this.r.current();
					var currentG = this.g.current();
					var currentB = this.b.current();
						
					var fill = rgbText(currentR, currentG, currentB);
					
					var radiusOuter;
					var lastChildAngle;
					var truncateWedge =
					(
						(this.hasChildren() || this == selectedNode ) &&
						! this.keyed &&
						(compress || depth < maxDisplayDepth) &&
						drawChildren
					);
					
					if ( truncateWedge )
					{
						radiusOuter = this.children.length ? this.children[0].radiusInner.current() * gRadius : radiusInner;
					}
					else
					{
						radiusOuter = gRadius;
					}
					/*
					if ( this.hasChildren() )
					{
						radiusOuter = this.children[0].getUncollapsed().radiusInner.current() * gRadius + 1;
					}
					else
					{ // TEMP
						radiusOuter = radiusInner + nodeRadius * gRadius;
						
						if ( radiusOuter > gRadius )
						{
							radiusOuter = gRadius;
						}
					}
					*/
					context.globalAlpha = alphaWedgeCurrent;
					
					if ( radiusInner != radiusOuter || truncateWedge )
					{
						drawWedge
						(
							angleStartCurrent,
							angleEndCurrent,
							radiusInner,
							radiusOuter,//this.radiusOuter.current() * gRadius,
							//'rgba(0, 200, 0, .1)',
							fill,
							this.alphaPattern.current()
						);
						
						if ( truncateWedge )
						{
							// fill in the extra space if the sum of our childrens'
							// magnitudes is less than ours
							
							if ( lastChildAngleEnd < angleEndCurrent )//&& false) // TEMP
							{
								if ( radiusOuter > 1 )
								{
									// overlap slightly to hide the seam
									
	//								radiusOuter -= 1;
								}
								
								if ( alphaWedgeCurrent < 1 )
								{
									context.globalAlpha = this.alphaOther.current();
									drawWedge
									(
										lastChildAngleEnd,
										angleEndCurrent,
										radiusOuter,
										gRadius,
										colorUnclassified,
										0
									);
									context.globalAlpha = alphaWedgeCurrent;
								}
								
								drawWedge
								(
									lastChildAngleEnd,
									angleEndCurrent,
									radiusOuter,
									gRadius,//this.radiusOuter.current() * gRadius,
									//'rgba(200, 0, 0, .1)',
									fill,
									this.alphaPattern.current()
								);
							}
						}
						
						if ( radiusOuter < gRadius )
						{
							// patch up the seam
							//
							context.beginPath();
							context.arc(0, 0, radiusOuter, angleStartCurrent/*lastChildAngleEnd*/, angleEndCurrent, false);
							context.strokeStyle = fill;
							context.lineWidth = 1;
							context.stroke();
						}
					}
					
					if ( this.keyed && selected && showKeys )//&& progress == 1 )
					{
						this.drawKey
						(
							(angleStartCurrent + angleEndCurrent) / 2,
							(
								this == highlightedNode ||
								this == focusNode ||
								this.searchResults
							),
							this == highlightedNode || this == focusNode
						);
					}
				}
			}
		}
		
		this.hiddenLabels = Array();
		
		if ( drawChildren )
		{
			// draw children
			//
			for ( var i = 0; i < this.children.length; i++ )
			{
				if ( this.drawHiddenChildren(i, selected, labelMode, searchHighlighted) )
				{
					i = this.children[i].hiddenEnd;
				}
				else
				{
					this.children[i].draw(labelMode, selected, searchHighlighted);
				}
			}
		}
	};
	
	this.drawHiddenChildren = function
	(
		firstHiddenChild,
		selected,
		labelMode,
		searchHighlighted
	)
	{
		var firstChild = this.children[firstHiddenChild];
		
		if ( firstChild.hiddenEnd == null || firstChild.radiusInner.current() == 1 )
		{
			return false;
		}
		
		for ( var i = firstHiddenChild; i < firstChild.hiddenEnd; i++ )
		{
			if ( ! this.children[i].hide || ! this.children[i].hidePrev && progress < 1 )
			{
				return false;
			}
		}
		
		var angleStart = firstChild.angleStart.current() + rotationOffset;
		var lastChild = this.children[firstChild.hiddenEnd];
		var angleEnd = lastChild.angleEnd.current() + rotationOffset;
		var radiusInner = gRadius * firstChild.radiusInner.current();
		var hiddenChildren = firstChild.hiddenEnd - firstHiddenChild + 1;
		
		if ( labelMode )
		{
			var hiddenSearchResults = 0;
			
			for ( var i = firstHiddenChild; i <= firstChild.hiddenEnd; i++ )
			{
				hiddenSearchResults += this.children[i].searchResults;
				
				if ( this.children[i].magnitude == 0 )
				{
					hiddenChildren--;
				}
			}
			
			if
			(
				selected &&
				(angleEnd - angleStart) * 
				(gRadius + gRadius) >=
				minWidth() ||
				this == highlightedNode &&
				hiddenChildren ||
				hiddenSearchResults
			)
			{
				context.globalAlpha = this.alphaWedge.current();
				
				this.drawHiddenLabel
				(
					angleStart,
					angleEnd,
					hiddenChildren,
					hiddenSearchResults
				);
			}
		}
		
		var drawWedges = true;
		
		for ( var i = firstHiddenChild; i <= firstChild.hiddenEnd; i++ )
		{
			// all hidden children must be completely hidden to draw together
			
			if ( this.children[i].alphaPattern.current() != this.children[i].alphaWedge.current() )
			{
				drawWedges = false;
				break;
			}
		}
		
		if ( labelMode )
		{
			if ( drawWedges )
			{
				var drawRadial = (angleEnd < this.angleEnd.current() + rotationOffset);
				this.drawLines(angleStart, angleEnd, radiusInner, drawRadial);
			}
			
			if ( hiddenSearchResults && ! searchHighlighted )
			{
				drawWedge
				(
					angleStart,
					angleEnd,
					radiusInner,
					gRadius,//this.radiusOuter.current() * gRadius,
					highlightFill,
					0,
					true
				);
			}
		}
		else if ( drawWedges )
		{
			context.globalAlpha = this.alphaWedge.current();
			
			var fill = rgbText
			(
				firstChild.r.current(),
				firstChild.g.current(),
				firstChild.b.current()
			);
			
			drawWedge
			(
				angleStart,
				angleEnd,
				radiusInner,
				gRadius,//this.radiusOuter.current() * gRadius,
				fill,
				context.globalAlpha,
				false
			);
		}
		
		return drawWedges;
	}
	
	this.drawHiddenLabel = function(angleStart, angleEnd, value, hiddenSearchResults)
	{
		var textAngle = (angleStart + angleEnd) / 2;
		var labelRadius = gRadius + fontSize;//(radiusInner + radius) / 2;
		
		var hiddenLabel = Array();
		
		hiddenLabel.value = value;
		hiddenLabel.angle = textAngle;
		hiddenLabel.search = hiddenSearchResults;
		
		this.hiddenLabels.push(hiddenLabel);
		
		drawTick(gRadius - fontSize * .75, fontSize * 1.5, textAngle);
		drawTextPolar
		(
			value.toString() + ' more',
			0, // inner text
			textAngle,
			labelRadius,
			true, // radial
			hiddenSearchResults, // bubble
			this == highlightedNode || this == focusNode, // bold
			false,
			hiddenSearchResults
		);
	}
	
	this.drawHighlight = function(bold)
	{
		var angleStartCurrent = this.angleStart.current() + rotationOffset;
		var angleEndCurrent = this.angleEnd.current() + rotationOffset;
		var radiusInner = this.radiusInner.current() * gRadius;
		
		//this.setHighlightStyle();
		
		if ( this == focusNode && this == highlightedNode && this.hasChildren() )
		{
//			context.fillStyle = "rgba(255, 255, 255, .3)";
			arrow
			(
				angleStartCurrent,
				angleEndCurrent,
				radiusInner
			);
		}
		else
		{
			drawWedge
			(
				angleStartCurrent,
				angleEndCurrent,
				radiusInner,
				gRadius,
				highlightFill,
				0,
				true
			);
		}
		
		// check if hidden children should be highlighted
		//
		for ( var i = 0; i < this.children.length; i++ )
		{
			if
			(
				this.children[i].getDepth() - selectedNode.getDepth() + 1 <=
				maxDisplayDepth &&
				this.children[i].hiddenEnd != null
			)
			{
				var firstChild = this.children[i];
				var lastChild = this.children[firstChild.hiddenEnd];
				var hiddenAngleStart = firstChild.angleStart.current() + rotationOffset;
				var hiddenAngleEnd = lastChild.angleEnd.current() + rotationOffset;
				var hiddenRadiusInner = gRadius * firstChild.radiusInner.current();
				
				drawWedge
				(
					hiddenAngleStart,
					hiddenAngleEnd,
					hiddenRadiusInner,
					gRadius,
					'rgba(255, 255, 255, .3)',
					0,
					true
				);
				
				if ( false && ! this.searchResults )
				{
					this.drawHiddenLabel
					(
						hiddenAngleStart,
						hiddenAngleEnd,
						firstChild.hiddenEnd - i + 1
					);
				}
				
				i = firstChild.hiddenEnd;
			}
		}
		
//			context.strokeStyle = 'black';
		context.fillStyle = 'black';
		
		var highlight = ! ( progress < 1 && zoomOut && this == selectedNodeLast );
		
		var angle = (angleEndCurrent + angleStartCurrent) / 2;
		
		if ( ! (this.keyed && showKeys) )
		{
			this.drawLabel(angle, true, bold, true, this.radial);
		}
	}
	
	this.drawHighlightCenter = function()
	{
		if ( ! this.canDisplayHistory() )
		{
			return;
		}
		
		context.lineWidth = highlightLineWidth;
		context.strokeStyle = 'black';
		context.fillStyle = "rgba(255, 255, 255, .6)";
		
		context.fillStyle = 'black';
		this.drawLabel(3 * Math.PI / 2, true, true, false);
		context.font = fontNormal;
	}
	
	this.drawKey = function(angle, highlight, bold)
	{
		var offset = keyOffset();
		var color;
		var colorText = this.magnitude == 0 ? 'gray' : 'black';
		var patternAlpha = this.alphaPattern.end;
		var boxLeft = imageWidth - keySize - margin;
		var textY = offset + keySize / 2;
		
		var label;
		var keyNameWidth;
		
		if ( this == selectedNode )
		{
			color = colorUnclassified;
			label =
				this.getUnclassifiedText() +
				'   ' +
				this.getUnclassifiedPercentage();
			keyNameWidth = measureText(label, false);
		}
		else
		{
			label = this.keyLabel;
			color = rgbText(this.r.end, this.g.end, this.b.end);
			
			if ( highlight )
			{
				if ( this.searchResultChildren() )
				{
					label = label + searchResultString(this.searchResultChildren());
				}
				
				keyNameWidth = measureText(label, bold);
			}
			else
			{
				keyNameWidth = this.keyNameWidth;
			}
		}
		
		var textLeft = boxLeft - keyBuffer - keyNameWidth - fontSize / 2;
		var labelLeft = textLeft;
		
		if ( labelLeft > keyMinTextLeft - fontSize / 2 )
		{
			keyMinTextLeft -= fontSize / 2;
			
			if ( keyMinTextLeft < centerX - gRadius + fontSize / 2 )
			{
				keyMinTextLeft = centerX - gRadius + fontSize / 2;
			}
			
			labelLeft = keyMinTextLeft;
		}
		
		var lineX = new Array();
		var lineY = new Array();
		
		var bendRadius;
		var keyAngle = Math.atan((textY - centerY) / (labelLeft - centerX));
		var arcAngle;
		
		if ( keyAngle < 0 )
		{
			keyAngle += Math.PI;
		}
		
		if ( keyMinAngle == 0 || angle < keyMinAngle )
		{
			keyMinAngle = angle;
		}
		
		if ( angle > Math.PI && keyMinAngle > Math.PI )
		{
			// allow lines to come underneath the chart
			
			angle -= Math.PI * 2;
		}
		
		lineX.push(Math.cos(angle) * gRadius);
		lineY.push(Math.sin(angle) * gRadius);
		
		if ( angle < keyAngle && textY > centerY + Math.sin(angle) * (gRadius + buffer * (currentKey - 1) / (keys + 1) / 2 + buffer / 2) )
		{
			bendRadius = gRadius + buffer - buffer * currentKey / (keys + 1) / 2;
		}
		else
		{
			bendRadius = gRadius + buffer * currentKey / (keys + 1) / 2 + buffer / 2;
		}
		
		var outside =
			Math.sqrt
			(
				Math.pow(labelLeft - centerX, 2) +
				Math.pow(textY - centerY, 2)
			) > bendRadius;
		
		if ( ! outside )
		{
			arcAngle = Math.asin((textY - centerY) / bendRadius);
			
			keyMinTextLeft = min(keyMinTextLeft, centerX + bendRadius * Math.cos(arcAngle) - fontSize / 2);
			
			if ( labelLeft < textLeft && textLeft > centerX + bendRadius * Math.cos(arcAngle) )
			{
				lineX.push(textLeft - centerX);
				lineY.push(textY - centerY);
			}
		}
		else
		{
			keyMinTextLeft = min(keyMinTextLeft, labelLeft - fontSize / 2);
			
			if ( angle < keyAngle )
			{
				// flip everything over y = x
				//
				arcAngle = Math.PI / 2 - keyLineAngle
				(
					Math.PI / 2 - angle,
					Math.PI / 2 - keyAngle,
					bendRadius,
					textY - centerY,
					labelLeft - centerX,
					lineY,
					lineX
				);
				
			}
			else
			{
				arcAngle = keyLineAngle
				(
					angle,
					keyAngle,
					bendRadius,
					labelLeft - centerX,
					textY - centerY,
					lineX,
					lineY
				);
			}
		}
		
		if ( labelLeft > centerX + bendRadius * Math.cos(arcAngle) ||
		textY > centerY + bendRadius * Math.sin(arcAngle) + .01)
//		if ( outside ||  )
		{
			lineX.push(labelLeft - centerX);
			lineY.push(textY - centerY);
			
			if ( textLeft != labelLeft )
			{
				lineX.push(textLeft - centerX);
				lineY.push(textY - centerY);
			}
		}
		
		context.globalAlpha = this.alphaWedge.current();
		
		if ( snapshotMode )
		{
			var labelSVG;
			
			if ( this == selectedNode )
			{
				labelSVG =
					this.getUnclassifiedText() +
					spacer() +
					this.getUnclassifiedPercentage();
			}
			else
			{
				labelSVG = this.name + spacer() + this.getPercentage() + '%';
			}
			
			svg +=
				'<rect fill="' + color + '" ' +
				'x="' + boxLeft + '" y="' + offset +
				'" width="' + keySize + '" height="' + keySize + '"/>';
			
			if ( patternAlpha )
			{
				svg +=
					'<rect fill="url(#hiddenPattern)" style="stroke:none" ' +
					'x="' + boxLeft + '" y="' + offset +
					'" width="' + keySize + '" height="' + keySize + '"/>';
			}
			
			svg +=
				'<path class="line' +
				(highlight ? ' highlight' : '') +
				'" d="M ' + (lineX[0] + centerX) + ',' +
				(lineY[0] + centerY);
			
			if ( angle != arcAngle )
			{
				svg +=
					' L ' + (centerX + bendRadius * Math.cos(angle)) + ',' +
					(centerY + bendRadius * Math.sin(angle)) +
					' A ' + bendRadius + ',' + bendRadius + ' 0 ' +
					'0,' + (angle > arcAngle ? '0' : '1') + ' ' +
					(centerX + bendRadius * Math.cos(arcAngle)) + ',' +
					(centerY + bendRadius * Math.sin(arcAngle));
			}
			
			for ( var i = 1; i < lineX.length; i++ )
			{
				svg +=
					' L ' + (centerX + lineX[i]) + ',' +
					(centerY + lineY[i]);
			}
			
			svg += '"/>';
			
			if ( highlight )
			{
				if ( this.searchResultChildren() )
				{
					labelSVG = labelSVG + searchResultString(this.searchResultChildren());
				}
				
				drawBubbleSVG
				(
					boxLeft - keyBuffer - keyNameWidth - fontSize / 2,
					textY - fontSize,
					keyNameWidth + fontSize,
					fontSize * 2,
					fontSize,
					0
				);
				
				if ( this.isSearchResult )
				{
					drawSearchHighlights
					(
						label,
						boxLeft - keyBuffer - keyNameWidth,
						textY,
						0
					)
				}
			}
			
			svg += svgText(labelSVG, boxLeft - keyBuffer, textY, 'end', bold, colorText);
		}
		else
		{
			context.fillStyle = color;
			context.translate(-centerX, -centerY);
			context.strokeStyle = 'black';
				context.globalAlpha = 1;//this.alphaWedge.current();
			
			context.fillRect(boxLeft, offset, keySize, keySize);
			
			if ( patternAlpha )
			{
				context.globalAlpha = patternAlpha;
				context.fillStyle = hiddenPattern;
				
				// make clipping box for Firefox performance
				context.beginPath();
				context.moveTo(boxLeft, offset);
				context.lineTo(boxLeft + keySize, offset);
				context.lineTo(boxLeft + keySize, offset + keySize);
				context.lineTo(boxLeft, offset + keySize);
				context.closePath();
				context.save();
				context.clip();
				
				context.fillRect(boxLeft, offset, keySize, keySize);
				context.fillRect(boxLeft, offset, keySize, keySize);
				
				context.restore(); // remove clipping region
			}
			
			if ( highlight )
			{
				this.setHighlightStyle();
				context.fillRect(boxLeft, offset, keySize, keySize);
			}
			else
			{
				context.lineWidth = thinLineWidth;
			}
			
			context.strokeRect(boxLeft, offset, keySize, keySize);
			
			if ( lineX.length )
			{
				context.beginPath();
				context.moveTo(lineX[0] + centerX, lineY[0] + centerY);
				
				context.arc(centerX, centerY, bendRadius, angle, arcAngle, angle > arcAngle);
				
				for ( var i = 1; i < lineX.length; i++ )
				{
					context.lineTo(lineX[i] + centerX, lineY[i] + centerY);
				}
				
				context.globalAlpha = this == selectedNode ?
					this.children[0].alphaWedge.current() :
					this.alphaWedge.current();
				context.lineWidth = highlight ? highlightLineWidth : thinLineWidth;
				context.stroke();
				context.globalAlpha = 1;
			}
			
			if ( highlight )
			{
				drawBubbleCanvas
				(
					boxLeft - keyBuffer - keyNameWidth - fontSize / 2,
					textY - fontSize,
					keyNameWidth + fontSize,
					fontSize * 2,
					fontSize,
					0
				);
				
				if ( this.isSearchResult )
				{
					drawSearchHighlights
					(
						label,
						boxLeft - keyBuffer - keyNameWidth,
						textY,
						0
					)
				}
			}
			
			drawText(label, boxLeft - keyBuffer, offset + keySize / 2, 0, 'end', bold, colorText);
			
			context.translate(centerX, centerY);
		}
		
		currentKey++;
	}
	
	this.drawLabel = function(angle, bubble, bold, selected, radial)
	{
		if ( context.globalAlpha == 0 )
		{
			return;
		}
		
		var innerText;
		var label;
		var radius;
		
		if ( radial )
		{
			radius = (this.radiusInner.current() + 1) * gRadius / 2;
		}
		else
		{
			radius = this.labelRadius.current() * gRadius;
		}
		
		if ( radial && (selected || bubble ) )
		{
			var percentage = this.getPercentage();
			innerText = percentage + '%';
		}
		
		if
		(
			! radial &&
			this != selectedNode &&
			! bubble &&
			( !zoomOut || this != selectedNodeLast)
		)
		{
			label = this.shortenLabel();
		}
		else
		{
			label = this.name;
		}
		
		if (showMagnitude)
		{
    		label += ' [' + this.magnitude + ']'
    	}
		
		var flipped = drawTextPolar
		(
			label,
			innerText,
			angle,
			radius,
			radial,
			bubble,
			bold,
//			this.isSearchResult && this.shouldAddSearchResultsString() && (!selected || this == selectedNode || highlight),
			this.isSearchResult && (!selected || this == selectedNode || bubble),
			(this.hideAlone || !selected || this == selectedNode ) ? this.searchResultChildren() : 0
		);
		
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
		
		if
		(
			! radial &&
			! bubble &&
			this != selectedNode &&
			this.angleEnd.end != this.angleStart.end &&
			nLabelOffsets[depth - 2] > 2 &&
			this.labelWidth.current() > (this.angleEnd.end - this.angleStart.end) * Math.abs(radius) &&
			! ( zoomOut && this == selectedNodeLast ) &&
			this.labelRadius.end > 0
		)
		{
			// name extends beyond wedge; draw tick mark towards the central
			// radius for easier identification
			
			var radiusCenter = compress ?
				(compressedRadii[depth - 1] + compressedRadii[depth - 2]) / 2 :
				(depth - .5) * nodeRadius;
			
			if ( this.labelRadius.end > radiusCenter )
			{
				if ( flipped )
				{
					drawTick(radius - tickLength * 1.4 , tickLength, angle);
				}
				else
				{
					drawTick(radius - tickLength * 1.7, tickLength, angle);
				}
			}
			else
			{
				if ( flipped )
				{
					drawTick(radius + tickLength * .7, tickLength, angle);
				}
				else
				{
					drawTick(radius + tickLength * .4, tickLength, angle);
				}
			}
		}
	}
	
	this.drawLines = function(angleStart, angleEnd, radiusInner, drawRadial, selected)
	{
		if ( snapshotMode )
		{
			if ( this != selectedNode)
			{
				if ( angleEnd == angleStart + Math.PI * 2 )
				{
					// fudge to prevent overlap, which causes arc ambiguity
					//
					angleEnd -= .1 / gRadius;
				}
				
				var longArc = angleEnd - angleStart > Math.PI ? 1 : 0;
				
				var x1 = centerX + radiusInner * Math.cos(angleStart);
				var y1 = centerY + radiusInner * Math.sin(angleStart);
				
				var x2 = centerX + gRadius * Math.cos(angleStart);
				var y2 = centerY + gRadius * Math.sin(angleStart);
				
				var x3 = centerX + gRadius * Math.cos(angleEnd);
				var y3 = centerY + gRadius * Math.sin(angleEnd);
				
				var x4 = centerX + radiusInner * Math.cos(angleEnd);
				var y4 = centerY + radiusInner * Math.sin(angleEnd);
				
				if ( this.alphaArc.end )
				{
					var dArray =
					[
						" M ", x4, ",", y4,
						" A ", radiusInner, ",", radiusInner, " 0 ", longArc,
							" 0 ", x1, ",", y1
					];
					
					svg += '<path class="line" d="' + dArray.join('') + '"/>';
				}
				
				if ( drawRadial && this.alphaLine.end )
				{
					svg += '<line x1="' + x3 + '" y1="' + y3 + '" x2="' + x4 + '" y2="' + y4 + '"/>';
				}
			}
		}
		else
		{
			context.lineWidth = thinLineWidth;
			context.strokeStyle = 'black';
			context.beginPath();
			context.arc(0, 0, radiusInner, angleStart, angleEnd, false);
			context.globalAlpha = this.alphaArc.current();
			context.stroke();
			
			if ( drawRadial )
			{
				var x1 = radiusInner * Math.cos(angleEnd);
				var y1 = radiusInner * Math.sin(angleEnd);
				var x2 = gRadius * Math.cos(angleEnd);
				var y2 = gRadius * Math.sin(angleEnd);
				
				context.beginPath();
				context.moveTo(x1, y1);
				context.lineTo(x2, y2);
				
//				if ( this.getCollapse() )//( selected && this != selectedNode )
				{
					context.globalAlpha = this.alphaLine.current();
				}
				
				context.stroke();
			}
		}
	}
	
	this.drawMap = function(child)
	{
		if ( this.parent )
		{
			this.parent.drawMap(child);
		}
		
		if ( this.getCollapse() && this != child || this == focusNode )
		{
			return;
		}
		
		var angleStart =
			(child.baseMagnitude - this.baseMagnitude) / this.magnitude * Math.PI * 2 +
			rotationOffset;
		var angleEnd =
			(child.baseMagnitude - this.baseMagnitude + child.magnitude) /
			this.magnitude * Math.PI * 2 +
			rotationOffset;
		
		var box = this.getMapPosition();
		
		context.save();
		context.fillStyle = 'black';
		context.textAlign = 'end';
		context.textBaseline = 'middle';
		
		var textX = box.x - mapRadius - mapBuffer;
		var percentage = getPercentage(child.magnitude / this.magnitude);
		
		var highlight = this == selectedNode || this == highlightedNode;
		
		if ( highlight )
		{
			context.font = fontBold;
		}
		else
		{
			context.font = fontNormal;
		}
		
		context.fillText(percentage + '% of', textX, box.y - mapRadius / 3);
		context.fillText(this.name, textX, box.y + mapRadius / 3);
		
		if ( highlight )
		{
			context.font = fontNormal;
		}
		
		if ( this == highlightedNode && this != selectedNode )
		{
			context.fillStyle = 'rgb(245, 245, 245)';
//			context.fillStyle = 'rgb(200, 200, 200)';
		}
		else
		{
			context.fillStyle = 'rgb(255, 255, 255)';
		}
		
		context.beginPath();
		context.arc(box.x, box.y, mapRadius, 0, Math.PI * 2, true);
		context.closePath();
		context.fill();
		
		if ( this == selectedNode )
		{
			context.lineWidth = 1;
			context.fillStyle = 'rgb(100, 100, 100)';
		}
		else
		{
			if ( this == highlightedNode )
			{
				context.lineWidth = .2;
				context.fillStyle = 'rgb(190, 190, 190)';
			}
			else
			{
				context.lineWidth = .2;
				context.fillStyle = 'rgb(200, 200, 200)';
			}
		}
		
		var maxDepth = this.getMaxDepth();
		
		if ( ! compress && maxDepth > maxPossibleDepth + this.getDepth() - 1 )
		{
			maxDepth = maxPossibleDepth + this.getDepth() - 1;
		}
		
		if ( this.getDepth() < selectedNode.getDepth() )
		{
			if ( child.getDepth() - 1 >= maxDepth )
			{
				maxDepth = child.getDepth();
			}
		}
		
		var radiusInner;
		
		if ( compress )
		{
			radiusInner = 0;
//				Math.atan(child.getDepth() - this.getDepth()) /
//				Math.PI * 2 * .9;
		}
		else
		{
			radiusInner =
				(child.getDepth() - this.getDepth()) /
				(maxDepth - this.getDepth() + 1);
		}
		
		context.stroke();
		context.beginPath();
		
		if ( radiusInner == 0 )
		{
			context.moveTo(box.x, box.y);
		}
		else
		{
			context.arc(box.x, box.y, mapRadius * radiusInner, angleEnd, angleStart, true);
		}
		
		context.arc(box.x, box.y, mapRadius, angleStart, angleEnd, false);
		context.closePath();
		context.fill();
		
		if ( this == highlightedNode && this != selectedNode )
		{
			context.lineWidth = 1;
			context.stroke();
		}
		
		context.restore();
	}
	
	this.drawReferenceRings = function(childRadiusInner)
	{
		if ( snapshotMode )
		{
			svg +=
				'<circle cx="' + centerX + '" cy="' + centerY +
				'" r="' + childRadiusInner + '"/>';
			svg +=
				'<circle cx="' + centerX + '" cy="' + centerY +
				'" r="' + gRadius + '"/>';
		}
		else
		{
			context.globalAlpha = 1 - this.alphaLine.current();//this.getUncollapsed().alphaLine.current();
			context.beginPath();
			context.arc(0, 0, childRadiusInner, 0, Math.PI * 2, false);
			context.stroke();
			context.beginPath();
			context.arc(0, 0, gRadius, 0, Math.PI * 2, false);
			context.stroke();
		}
	}
	
	this.getCollapse = function()
	{
		return (
			collapse &&
			this.collapse &&
			this.depth != maxAbsoluteDepth
			);
	}
	
	this.getDepth = function()
	{
		if ( collapse )
		{
			return this.depthCollapsed;
		}
		else
		{
			return this.depth;
		}
	}
	
	this.getMagnitude = function()
	{
		return this.attributes[magnitudeIndex][currentDataset];
	}
	
	this.getMapPosition = function()
	{
		return {
			x : (details.offsetLeft + details.clientWidth - mapRadius),
			y : ((focusNode.getDepth() - this.getDepth()) *
				(mapBuffer + mapRadius * 2) - mapRadius) +
				details.clientHeight + details.offsetTop
		};
	}
	
	this.getMaxDepth = function(limit)
	{
		var max;
		
		if ( collapse )
		{
			return this.maxDepthCollapsed;
		}
		else
		{
			if ( this.maxDepth > maxAbsoluteDepth )
			{
				return maxAbsoluteDepth;
			}
			else
			{
				return this.maxDepth;
			}
		}
	}
	
	this.getData = function(index, summary)
	{
		var files = new Array();
		
		if
		(
			this.attributes[index] != null &&
			this.attributes[index][currentDataset] != null &&
			this.attributes[index][currentDataset] != ''
		)
		{
			files.push
			(
				document.location +
				'.files/' +
				this.attributes[index][currentDataset]
			);
		}
		
		if ( summary )
		{
			for ( var i = 0; i < this.children.length; i++ )
			{
				files = files.concat(this.children[i].getData(index, true));
			}
		}
		
		return files;
	}
	
	this.getList = function(index, summary)
	{
		var list;
		
		if
		(
			this.attributes[index] != null &&
			this.attributes[index][currentDataset] != null
		)
		{
			list = this.attributes[index][currentDataset];
		}
		else
		{
			list = new Array();
		}
		
		if ( summary )
		{
			for ( var i = 0; i < this.children.length; i++ )
			{
				list = list.concat(this.children[i].getList(index, true));
			}
		}
		
		return list;
	}
	
	this.getParent = function()
	{
		// returns parent, accounting for collapsing or 0 if doesn't exist
		
		var parent = this.parent;
		
		while ( parent != 0 && parent.getCollapse() )
		{
			parent = parent.parent;
		}
		
		return parent;
	}
	
	this.getPercentage = function()
	{
		return getPercentage(this.magnitude / selectedNode.magnitude);
	}
	
	this.getUnclassifiedPercentage = function()
	{
		if ( this.children.length )
		{
			var lastChild = this.children[this.children.length - 1];
		
			return getPercentage
			(
				(
					this.baseMagnitude +
					this.magnitude -
					lastChild.magnitude -
					lastChild.baseMagnitude
				) / this.magnitude
			) + '%';
		}
		else
		{
			return '100%';
		}
	}
	
	this.getUnclassifiedText = function()
	{
		return '[other '+ this.name + ']';
	}
	
	this.getUncollapsed = function()
	{
		// recurse through collapsed children until uncollapsed node is found
		
		if ( this.getCollapse() )
		{
			return this.children[0].getUncollapsed();
		}
		else
		{
			return this;
		}
	}
	
	this.hasChildren = function()
	{
		return this.children.length && this.depth < maxAbsoluteDepth && this.magnitude;
	}
	
	this.hasParent = function(parent)
	{
		if ( this.parent )
		{
			if ( this.parent == parent )
			{
				return true;
			}
			else
			{
				return this.parent.hasParent(parent);
			}
		}
		else
		{
			return false;
		}
	}
	
	this.maxVisibleDepth = function(maxDepth)
	{
		var childInnerRadius;
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
		var currentMaxDepth = depth;
		
		if ( this.hasChildren() && depth < maxDepth)
		{
			var lastChild = this.children[this.children.length - 1];
			
			if ( this.name == 'Pseudomonadaceae' )
			{
				var x = 3;
			}
			
			if
			(
				lastChild.baseMagnitude + lastChild.magnitude <
				this.baseMagnitude + this.magnitude
			)
			{
				currentMaxDepth++;
			}
			
			if ( compress )
			{
				childInnerRadius = compressedRadii[depth - 1];
			}
			else
			{
				childInnerRadius = (depth) / maxDepth;
			}
			
			for ( var i = 0; i < this.children.length; i++ )
			{
				if
				(//true ||
					this.children[i].magnitude *
					angleFactor *
					(childInnerRadius + 1) *
					gRadius >=
					minWidth()
				)
				{
					var childMaxDepth = this.children[i].maxVisibleDepth(maxDepth);
					
					if ( childMaxDepth > currentMaxDepth )
					{
						currentMaxDepth = childMaxDepth;
					}
				}
			}
		}
		
		return currentMaxDepth;
	}
	
	this.resetLabelWidth = function()
	{
		var nameWidthOld = this.nameWidth;
		
		if ( true || ! this.radial )//&& fontSize != fontSizeLast )
		{
			var dim = context.measureText(this.name);
			this.nameWidth = dim.width;
		}
		
		if ( fontSize != fontSizeLast && this.labelWidth.end == nameWidthOld * labelWidthFudge )
		{
			// font size changed; adjust start of tween to match
			
			this.labelWidth.start = this.nameWidth * labelWidthFudge;
		}
		else
		{
			this.labelWidth.start = this.labelWidth.current();
		}
		
		this.labelWidth.end = this.nameWidth * labelWidthFudge;
	}
	
	this.restrictLabelWidth = function(width)
	{
		if ( width < this.labelWidth.end )
		{
			this.labelWidth.end = width;
		}
	}
	
	this.search = function()
	{
		this.isSearchResult = false;
		this.searchResults = 0;
		
		if
		(
			! this.getCollapse() &&
			search.value != '' &&
			this.name.toLowerCase().indexOf(search.value.toLowerCase()) != -1
		)
		{
			this.isSearchResult = true;
			this.searchResults = 1;
			nSearchResults++;
		}
		
		for ( var i = 0; i < this.children.length; i++ )
		{
			this.searchResults += this.children[i].search();
		}
		
		return this.searchResults;
	}
	
	this.searchResultChildren = function()
	{
		if ( this.isSearchResult )
		{
			return this.searchResults - 1;
		}
		else
		{
			return this.searchResults;
		}
	}
	
	this.setDepth = function(depth, depthCollapsed)
	{
		this.depth = depth;
		this.depthCollapsed = depthCollapsed;
		
		if
		(
			this.children.length == 1 &&
//			this.magnitude > 0 &&
			this.children[0].magnitude == this.magnitude &&
			( head.children.length > 1 || this.children[0].children.length )
		)
		{
			this.collapse = true;
		}
		else
		{
			this.collapse = false;
			depthCollapsed++;
		}
		
		for ( var i = 0; i < this.children.length; i++ )
		{
			this.children[i].setDepth(depth + 1, depthCollapsed);
		}
	}
	
	this.setHighlightStyle = function()
	{
		context.lineWidth = highlightLineWidth;
		
		if ( this.hasChildren() || this != focusNode || this != highlightedNode )
		{
			context.strokeStyle = 'black';
			context.fillStyle = "rgba(255, 255, 255, .3)";
		}
		else
		{
			context.strokeStyle = 'rgb(90,90,90)';
			context.fillStyle = "rgba(155, 155, 155, .3)";
		}
	}
	
	this.setLabelWidth = function(node)
	{
		if ( ! shorten || this.radial )
		{
			return; // don't need to set width
		}
		
		if ( node.hide )
		{
			alert('wtf');
			return;
		}
		
		var angle = (this.angleStart.end + this.angleEnd.end) / 2;
		var a; // angle difference
		
		if ( node == selectedNode )
		{
			a = Math.abs(angle - node.angleOther);
		}
		else
		{
			a = Math.abs(angle - (node.angleStart.end + node.angleEnd.end) / 2);
		}
		
		if ( a == 0 )
		{
			return;
		}
		
		if ( a > Math.PI )
		{
			a = 2 * Math.PI - a;
		}
		
		if ( node.radial || node == selectedNode )
		{
			var nodeLabelRadius;
			
			if ( node == selectedNode )
			{
				// radial 'other' label
				
				nodeLabelRadius = (node.children[0].radiusInner.end + 1) / 2;
			}
			else
			{
				nodeLabelRadius = (node.radiusInner.end + 1) / 2;
			}
			
			if ( a < Math.PI / 2 )
			{
				var r = this.labelRadius.end * gRadius + .5 * fontSize
				var hypotenuse = r / Math.cos(a);
				var opposite = r * Math.tan(a);
				var fontRadius = .8 * fontSize;
				
				if
				(
					nodeLabelRadius * gRadius < hypotenuse &&
					this.labelWidth.end / 2 + fontRadius > opposite
				)
				{
					this.labelWidth.end = 2 * (opposite - fontRadius);
				}
			}
		}
		else if
		(
			this.labelRadius.end == node.labelRadius.end &&
			a < Math.PI / 4
		)
		{
			// same radius with small angle; use circumferential approximation
			
			var dist = a * this.labelRadius.end * gRadius - fontSize * (1 - a * 4 / Math.PI) * 1.3;
			
			if ( this.labelWidth.end < dist )
			{
				node.restrictLabelWidth((dist - this.labelWidth.end / 2) * 2);
			}
			else if ( node.labelWidth.end < dist )
			{
				this.restrictLabelWidth((dist - node.labelWidth.end / 2) * 2);
			}
			else
			{
				// both labels reach halfway point; restrict both
				
				this.labelWidth.end = dist;
				node.labelWidth.end = dist
			}
		}
		else
		{
			var r1 = this.labelRadius.end * gRadius;
			var r2 = node.labelRadius.end * gRadius;
			
			// first adjust the radii to account for the height of the font by shifting them
			// toward each other
			//
			var fontFudge = .35 * fontSize;
			//
			if ( this.labelRadius.end < node.labelRadius.end )
			{
				r1 += fontFudge;
				r2 -= fontFudge;
			}
			else if ( this.labelRadius.end > node.labelRadius.end )
			{
				r1 -= fontFudge;
				r2 += fontFudge;
			}
			else
			{
				r1 -= fontFudge;
				r2 -= fontFudge;
			}
			
			var r1s = r1 * r1;
			var r2s = r2 * r2;
			
			// distance between the centers of the two labels
			//
			var dist = Math.sqrt(r1s + r2s - 2 * r1 * r2 * Math.cos(a));
			
			// angle at our label center between our radius and the line to the other label center
			//
			var b = Math.acos((r1s + dist * dist - r2s) / (2 * r1 * dist));
			
			// distance from our label center to the intersection of the two tangents
			//
			var l1 = Math.sin(a + b - Math.PI / 2) * dist / Math.sin(Math.PI - a);
			
			// distance from other label center the the intersection of the two tangents
			//
			var l2 = Math.sin(Math.PI / 2 - b) * dist / Math.sin(Math.PI - a);
			
			l1 = Math.abs(l1) - .4 * fontSize;
			l2 = Math.abs(l2) - .4 * fontSize;
/*			
			// amount to shorten the distances because of the height of the font
			//
			var l3 = 0;
			var fontRadius = fontSize * .55;
			//
			if ( l1 < 0 || l2 < 0 )
			{
				var l4 = fontRadius / Math.tan(a);
			l1 = Math.abs(l1);
			l2 = Math.abs(l2);
			
				l1 -= l4;
				l2 -= l4;
			}
			else
			{
				var c = Math.PI - a;
				
				l3 = fontRadius * Math.tan(c / 2);
			}
*/			
			if ( this.labelWidth.end / 2 > l1 && node.labelWidth.end / 2 > l2 )
			{
				// shorten the farthest one from the intersection
				
				if ( l1 > l2 )
				{
					this.restrictLabelWidth(2 * (l1));// - l3 - fontRadius));
				}
				else
				{
					node.restrictLabelWidth(2 * (l2));// - l3 - fontRadius));
				}
			}/*
			else if ( this.labelWidth.end / 2 > l1 + l3 && node.labelWidth.end / 2 > l2 - l3 )
			{
				node.restrictLabelWidth(2 * (l2 - l3));
			}
			else if ( this.labelWidth.end / 2 > l1 - l3 && node.labelWidth.end / 2 > l2 + l3 )
			{
				this.restrictLabelWidth(2 * (l1 - l3));
			}*/
		}
	}
	
	this.setMagnitudes = function(baseMagnitude)
	{
		this.magnitude = this.getMagnitude();
		this.baseMagnitude = baseMagnitude;
		
		for ( var i = 0; i < this.children.length; i++ )
		{
			this.children[i].setMagnitudes(baseMagnitude);
			baseMagnitude += this.children[i].magnitude;
		}
		
		this.maxChildMagnitude = baseMagnitude;
	}
	
	this.setMaxDepths = function()
	{
		this.maxDepth = this.depth;
		this.maxDepthCollapsed = this.depthCollapsed;
		
		for ( i in this.children )
		{
			var child = this.children[i];
			
			child.setMaxDepths();
			
			if ( child.maxDepth > this.maxDepth )
			{
				this.maxDepth = child.maxDepth;
			}
			
			if
			(
				child.maxDepthCollapsed > this.maxDepthCollapsed &&
				(child.depth <= maxAbsoluteDepth || maxAbsoluteDepth == 0)
			)
			{
				this.maxDepthCollapsed = child.maxDepthCollapsed;
			}
		}
	}
	
	this.setTargetLabelRadius = function()
	{
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
		var index = depth - 2;
		var labelOffset = labelOffsets[index];
		
		if ( this.radial )
		{
			//this.labelRadius.setTarget((this.radiusInner.end + 1) / 2);
			var max =
				depth == maxDisplayDepth ?
				1 :
				compressedRadii[index + 1];
			
			this.labelRadius.setTarget((compressedRadii[index] + max) / 2);
		}
		else
		{
			var radiusCenter;
			var width;
			
			if ( compress )
			{
				if ( nLabelOffsets[index] > 1 )
				{
					this.labelRadius.setTarget
					(
						lerp
						(
							labelOffset + .75,
							0,
							nLabelOffsets[index] + .5,
							compressedRadii[index],
							compressedRadii[index + 1]
						)
					);
				}
				else
				{
					this.labelRadius.setTarget((compressedRadii[index] + compressedRadii[index + 1]) / 2);
				}
			}
			else
			{
				radiusCenter =
					nodeRadius * (depth - 1) +
					nodeRadius / 2;
				width = nodeRadius;
				
				this.labelRadius.setTarget
				(
					radiusCenter + width * ((labelOffset + 1) / (nLabelOffsets[index] + 1) - .5)
				);
			}
		}
		
		if ( ! this.hide && ! this.keyed && nLabelOffsets[index] )
		{
			// check last and first labels in each track for overlap
			
			for ( var i = 0; i < maxDisplayDepth - 1; i++ )
			{
				for ( var j = 0; j <= nLabelOffsets[i]; j++ )
				{
					var last = labelLastNodes[i][j];
					var first = labelFirstNodes[i][j];
					
					if ( last )
					{
						if ( j == nLabelOffsets[i] )
						{
							// last is radial
							this.setLabelWidth(last);
						}
						else
						{
							last.setLabelWidth(this);
						}
					}
					
					if ( first )
					{
						if ( j == nLabelOffsets[i] )
						{
							this.setLabelWidth(first);
						}
						else
						{
							first.setLabelWidth(this);
						}
					}
				}
			}
			
			if ( selectedNode.canDisplayLabelOther )
			{
				this.setLabelWidth(selectedNode); // in case there is an 'other' label
			}
			
			if ( this.radial )
			{
				// use the last 'track' of this depth for radial
				
				labelLastNodes[index][nLabelOffsets[index]] = this;
				
				if ( labelFirstNodes[index][nLabelOffsets[index]] == 0 )
				{
					labelFirstNodes[index][nLabelOffsets[index]] = this;
				}
			}
			else
			{
				labelLastNodes[index][labelOffset] = this;
				
				// update offset
				
				labelOffsets[index] += 1;
				
				if ( labelOffsets[index] > nLabelOffsets[index] )
				{
					labelOffsets[index] -= nLabelOffsets[index];
					
					if ( !(nLabelOffsets[index] & 1) )
					{
						labelOffsets[index]--;
					}
				}
				else if ( labelOffsets[index] == nLabelOffsets[index] )
				{
					labelOffsets[index] -= nLabelOffsets[index];
					
					if ( false && !(nLabelOffsets[index] & 1) )
					{
						labelOffsets[index]++;
					}
				}
				
				if ( labelFirstNodes[index][labelOffset] == 0 )
				{
					labelFirstNodes[index][labelOffset] = this;
				}
			}
		}
		else if ( this.hide )
		{
			this.labelWidth.end = 0;
		}
	}
	
	this.setTargets = function()
	{
		if ( this == selectedNode )
		{
			this.setTargetsSelected
			(
				0,
				1,
				lightnessBase,
				false,
				false
			);
			return;
		}
		
		var depthRelative = this.getDepth() - selectedNode.getDepth();
		
		var parentOfSelected = selectedNode.hasParent(this);
/*		(
//			! this.getCollapse() &&
			this.baseMagnitude <= selectedNode.baseMagnitude &&
			this.baseMagnitude + this.magnitude >=
			selectedNode.baseMagnitude + selectedNode.magnitude
		);
*/		
		if ( parentOfSelected )
		{
			this.resetLabelWidth();
		}
		else
		{
			//context.font = fontNormal;
			var dim = context.measureText(this.name);
			this.nameWidth = dim.width;
			//this.labelWidth.setTarget(this.labelWidth.end);
			this.labelWidth.setTarget(0);
		}
		
		// set angles
		//
		if ( this.baseMagnitude <= selectedNode.baseMagnitude )
		{
			this.angleStart.setTarget(0);
		}
		else
		{
			this.angleStart.setTarget(Math.PI * 2);
		}
		//
		if
		(
			parentOfSelected ||
			this.baseMagnitude + this.magnitude >=
			selectedNode.baseMagnitude + selectedNode.magnitude
		)
		{
			this.angleEnd.setTarget(Math.PI * 2);
		}
		else
		{
			this.angleEnd.setTarget(0);
		}
		
		// children
		//
		for ( var i = 0; i < this.children.length; i++ )
		{
			this.children[i].setTargets();
		}
		
		if ( this.getDepth() <= selectedNode.getDepth() )
		{
			// collapse in
			
			this.radiusInner.setTarget(0);
			
			if ( parentOfSelected )
			{
				this.labelRadius.setTarget
				(
					(depthRelative) *
					historySpacingFactor * fontSize / gRadius
				);
				//this.scale.setTarget(1 - (selectedNode.getDepth() - this.getDepth()) / 18); // TEMP
			}
			else
			{
				this.labelRadius.setTarget(0);
				//this.scale.setTarget(1); // TEMP
			}
		}
		else if ( depthRelative + 1 > maxDisplayDepth )
		{
			// collapse out
			
			this.radiusInner.setTarget(1);
			this.labelRadius.setTarget(1);
			//this.scale.setTarget(1); // TEMP
		}
		else
		{
			// don't collapse
			
			if ( compress )
			{
				this.radiusInner.setTarget(compressedRadii[depthRelative - 1]);
			}
			else
			{
				this.radiusInner.setTarget(nodeRadius * (depthRelative));
			}
			
			//this.scale.setTarget(1); // TEMP
			
			if ( this == selectedNode )
			{
				this.labelRadius.setTarget(0);
			}
			else
			{
				if ( compress )
				{
					this.labelRadius.setTarget
					(
						(compressedRadii[depthRelative - 1] + compressedRadii[depthRelative]) / 2
					);
				}
				else
				{
					this.labelRadius.setTarget(nodeRadius * (depthRelative) + nodeRadius / 2);
				}
			}
		}
		
//		this.r.start = this.r.end;
//		this.g.start = this.g.end;
//		this.b.start = this.b.end;
		
		this.r.setTarget(255);
		this.g.setTarget(255);
		this.b.setTarget(255);

		this.alphaLine.setTarget(0);
		this.alphaArc.setTarget(0);
		this.alphaWedge.setTarget(0);
		this.alphaPattern.setTarget(0);
		this.alphaOther.setTarget(0);
		
		if ( parentOfSelected && ! this.getCollapse() )
		{
			var alpha =
			(
				1 -
				(selectedNode.getDepth() - this.getDepth()) /
				(Math.floor((compress ? compressedRadii[0] : nodeRadius) * gRadius / (historySpacingFactor * fontSize) - .5) + 1)
			);
			
			if ( alpha < 0 )
			{
				alpha = 0;
			}
			
			this.alphaLabel.setTarget(alpha);
			this.radial = false;
		}
		else
		{
			this.alphaLabel.setTarget(0);
		}
		
		this.hideAlonePrev = this.hideAlone;
		this.hidePrev = this.hide;
		
		if ( parentOfSelected )
		{
			this.hideAlone = false;
			this.hide = false;
		}
		
		if ( this.getParent() == selectedNode.getParent() )
		{
			this.hiddenEnd = null;
		}
		
		this.radialPrev = this.radial;
	}
	
	this.setTargetsSelected = function(hueMin, hueMax, lightness, hide, nextSiblingHidden)
	{
		var collapse = this.getCollapse();
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
		var canDisplayChildLabels = false;
		var lastChild;
		
		if ( this.hasChildren() )//&& ! hide )
		{
			lastChild = this.children[this.children.length - 1];
			this.hideAlone = true;
		}
		else
		{
			this.hideAlone = false;
		}
		
		// set child wedges
		//
		for ( var i = 0; i < this.children.length; i++ )
		{
			this.children[i].setTargetWedge();
			
			if
			(
				! this.children[i].hide &&
				( collapse || depth < maxDisplayDepth ) &&
				this.depth < maxAbsoluteDepth
			)
			{
				canDisplayChildLabels = true;
				this.hideAlone = false;
			}
		}
		
		if ( this == selectedNode || lastChild && lastChild.angleEnd.end < this.angleEnd.end - .01)
		{
			this.hideAlone = false;
		}
		
		if ( this.hideAlonePrev == undefined )
		{
			this.hideAlonePrev = this.hideAlone;
		}
		
		if ( this == selectedNode )
		{
			var otherArc = 
				this.children.length ?
					angleFactor *
					(
						this.baseMagnitude + this.magnitude -
						lastChild.baseMagnitude - lastChild.magnitude
					)
				: this.baseMagnitude + this.magnitude;
			this.canDisplayLabelOther =
				this.children.length ?
					otherArc *
					(this.children[0].radiusInner.end + 1) * gRadius >=
					minWidth()
				: true;
			
			this.keyUnclassified = false;
			
			if ( this.canDisplayLabelOther )
			{
				this.angleOther = Math.PI * 2 - otherArc / 2;
			}
			else if ( otherArc > 0.0000000001 )
			{
				this.keyUnclassified = true;
				keys++;
			}
			
			this.angleStart.setTarget(0);
			this.angleEnd.setTarget(Math.PI * 2);
			
			if ( this.children.length )
			{
				this.radiusInner.setTarget(0);
			}
			else
			{
				this.radiusInner.setTarget(compressedRadii[0]);
			}
			
			this.hidePrev = this.hide;
			this.hide = false;
			this.hideAlonePrev = this.hideAlone;
			this.hideAlone = false;
			this.keyed = false;
		}
		
		if ( hueMax - hueMin > 1 / 12 )
		{
			hueMax = hueMin + 1 / 12;
		}
		
		// set lightness
		//
		if ( ! ( hide || this.hideAlone ) )
		{
			if ( useHue() )
			{
				lightness = (lightnessBase + lightnessMax) / 2;
			}
			else
			{
				lightness = lightnessBase + (depth - 1) * lightnessFactor;
				
				if ( lightness > lightnessMax )
				{
					lightness = lightnessMax;
				}
			}
		}
		
		if ( hide )
		{
			this.hide = true;
		}
		
		if ( this.hidePrev == undefined )
		{
			this.hidePrev = this.hide;
		}
		
		var hiddenStart = -1;
		var hiddenHueNumer = 0;
		var hiddenHueDenom = 0;
		var i = 0;
		
		if ( ! this.hide )
		{
			this.hiddenEnd = null;
		}
		
		while ( true )
		{
			if ( ! this.hideAlone && ! hide && ( i == this.children.length || ! this.children[i].hide ) )
			{
				// reached a non-hidden child or the end; set targets for
				// previous group of hidden children (if any) using their
				// average hue
				
				if ( hiddenStart != -1 )
				{
					var hiddenHue = hiddenHueDenom ? hiddenHueNumer / hiddenHueDenom : hueMin;
					
					for ( var j = hiddenStart; j < i; j++ )
					{
						this.children[j].setTargetsSelected
						(
							hiddenHue,
							null,
							lightness,
							false,
							j < i - 1
						);
						
						this.children[j].hiddenEnd = null;
					}
					
					this.children[hiddenStart].hiddenEnd = i - 1;
				}
			}
			
			if ( i == this.children.length )
			{
				break;
			}
			
			var child = this.children[i];
			var childHueMin;
			var childHueMax;
			
			if ( this.magnitude > 0 && ! this.hide && ! this.hideAlone )
			{
				if ( useHue() )
				{
					childHueMin = child.hues[currentDataset];
				}
				else if ( this == selectedNode )
				{
					var min = 0.0;
					var max = 1.0;
					
					if ( this.children.length > 6 )
					{
						childHueMin = lerp((1 - Math.pow(1 - i / this.children.length, 1.4)) * .95, 0, 1, min, max);
						childHueMax = lerp((1 - Math.pow(1 - (i + .55) / this.children.length, 1.4)) * .95, 0, 1, min, max);
					}
					else
					{
						childHueMin = lerp(i / this.children.length, 0, 1, min, max);
						childHueMax = lerp((i + .55) / this.children.length, 0, 1, min, max);
					}
				}
				else
				{
					childHueMin = lerp
					(
						child.baseMagnitude,
						this.baseMagnitude, 
						this.baseMagnitude + this.magnitude,
						hueMin,
						hueMax
					);
					childHueMax = lerp
					(
						child.baseMagnitude + child.magnitude * .99,
						this.baseMagnitude,
						this.baseMagnitude + this.magnitude,
						hueMin,
						hueMax
					);
				}
			}
			else
			{
				childHueMin = hueMin;
				childHueMax = hueMax;
			}
			
			if ( ! this.hideAlone && ! hide && ! this.hide && child.hide )
			{
				if ( hiddenStart == -1 )
				{
					hiddenStart = i;
				}
				
				if ( useHue() )
				{
					hiddenHueNumer += childHueMin * child.magnitude;
					hiddenHueDenom += child.magnitude;
				}
				else
				{
					hiddenHueNumer += childHueMin;
					hiddenHueDenom++;
				}
			}
			else
			{
				hiddenStart = -1;
				
				this.children[i].setTargetsSelected
				(
					childHueMin,
					childHueMax,
					lightness,
					hide || this.keyed || this.hideAlone || this.hide && ! collapse,
					false
				);
			}
			
			i++;
		}
		
	 	if ( this.hue && this.magnitude )
	 	{
		 	this.hue.setTarget(this.hues[currentDataset]);
			
			if ( this.attributes[magnitudeIndex][lastDataset] == 0 )
			{
				this.hue.start = this.hue.end;
			}
		}
	 	
		this.radialPrev = this.radial;
		
		if ( this == selectedNode )
		{
			this.resetLabelWidth();
			this.labelWidth.setTarget(this.nameWidth * labelWidthFudge);
			this.alphaWedge.setTarget(0);
			this.alphaLabel.setTarget(1);
			this.alphaOther.setTarget(1);
			this.alphaArc.setTarget(0);
			this.alphaLine.setTarget(0);
			this.alphaPattern.setTarget(0);
			this.r.setTarget(255);
			this.g.setTarget(255);
			this.b.setTarget(255);
			this.radial = false;
			this.labelRadius.setTarget(0);
		}
		else
		{
			var rgb = hslToRgb
			(
				hueMin,
				saturation,
				lightness
			);
			
			this.r.setTarget(rgb.r);
			this.g.setTarget(rgb.g);
			this.b.setTarget(rgb.b);
			this.alphaOther.setTarget(0);
			
			this.alphaWedge.setTarget(1);
			
			if ( this.hide || this.hideAlone )
			{
				this.alphaPattern.setTarget(1);
			}
			else
			{
				this.alphaPattern.setTarget(0);
			}
			
			// set radial
			//
			if ( ! ( hide || this.hide ) )//&& ! this.keyed )
			{
				if ( this.hideAlone )
				{
					this.radial = true;
				}
				else if ( false && canDisplayChildLabels )
				{
					this.radial = false;
				}
				else
				{
					this.radial = true;
					
					if ( this.hasChildren() && depth < maxDisplayDepth )
					{
						var lastChild = this.children[this.children.length - 1];
						
						if
						(
							lastChild.angleEnd.end == this.angleEnd.end ||
							(
								(this.angleStart.end + this.angleEnd.end) / 2 -
								lastChild.angleEnd.end
							) * (this.radiusInner.end + 1) * gRadius * 2 <
							minWidth()
						)
						{
							this.radial = false;
						}
					}
				}
			}
			
			// set alphaLabel
			//
			if
			(
				collapse ||
				hide ||
				this.hide ||
				this.keyed ||
				depth > maxDisplayDepth ||
				! this.canDisplayDepth()
			)
			{
				this.alphaLabel.setTarget(0);
			}
			else
			{
				if
				(
					(this.radial || nLabelOffsets[depth - 2])
				)
				{
					this.alphaLabel.setTarget(1);
				}
				else
				{
					this.alphaLabel.setTarget(0);
					
					if ( this.radialPrev )
					{
						this.alphaLabel.start = 0;
					}
				}
			}
			
			// set alphaArc
			//
			if
			(
				collapse ||
				hide ||
				depth > maxDisplayDepth ||
				! this.canDisplayDepth()
			)
			{
				this.alphaArc.setTarget(0);
			}
			else
			{
				this.alphaArc.setTarget(1);
			}
			
			// set alphaLine
			//
			if
			(
				hide ||
				this.hide && nextSiblingHidden ||
				depth > maxDisplayDepth ||
				! this.canDisplayDepth()
			)
			{
				this.alphaLine.setTarget(0);
			}
			else
			{
				this.alphaLine.setTarget(1);
			}
			
			//if (  ! this.radial )
			{
				this.resetLabelWidth();
			}
			
			// set labelRadius target
			//
			if ( collapse )
			{
				this.labelRadius.setTarget(this.radiusInner.end);
			}
			else
			{
				if ( depth > maxDisplayDepth || ! this.canDisplayDepth() )
				{
					this.labelRadius.setTarget(1);
				}
				else
				{
					this.setTargetLabelRadius();
				}
			}
		}
	}
	
	this.setTargetWedge = function()
	{
		var depth = this.getDepth() - selectedNode.getDepth() + 1;
		
		// set angles
		//
		var baseMagnitudeRelative = this.baseMagnitude - selectedNode.baseMagnitude;
		//
		this.angleStart.setTarget(baseMagnitudeRelative * angleFactor);
		this.angleEnd.setTarget((baseMagnitudeRelative + this.magnitude) * angleFactor);
		
		// set radiusInner
		//
		if ( depth > maxDisplayDepth || ! this.canDisplayDepth() )
		{
			this.radiusInner.setTarget(1);
		}
		else
		{
			if ( compress )
			{
				this.radiusInner.setTarget(compressedRadii[depth - 2]);
			}
			else
			{
				this.radiusInner.setTarget(nodeRadius * (depth - 1));
			}
		}
		
		if ( this.hide != undefined )
		{
			this.hidePrev = this.hide;
		}
		
		if ( this.hideAlone != undefined )
		{
			this.hideAlonePrev = this.hideAlone;
		}
		
		// set hide
		//
		if
		(
			(this.angleEnd.end - this.angleStart.end) *
			(this.radiusInner.end * gRadius + gRadius) <
			minWidth()
		)
		{
			if ( depth == 2 && ! this.getCollapse() && this.depth <= maxAbsoluteDepth )
			{
				this.keyed = true;
				keys++;
				this.hide = false;
				
				var percentage = this.getPercentage();
				this.keyLabel = this.name + '   ' + percentage + '%';
				var dim = context.measureText(this.keyLabel);
				this.keyNameWidth = dim.width;
			}
			else
			{
				this.keyed = false;
				this.hide = depth > 2;
			}
		}
		else
		{
			this.keyed = false;
			this.hide = false;
		}
	}
	
	this.shortenLabel = function()
	{
		var label = this.name;
		
		var labelWidth = this.nameWidth;
		var maxWidth = this.labelWidth.current();
		var minEndLength = 0;
		
		if ( labelWidth > maxWidth && label.length > minEndLength * 2 )
		{
			var endLength =
				Math.floor((label.length - 1) * maxWidth / labelWidth / 2);
			
			if ( endLength < minEndLength )
			{
				endLength = minEndLength;
			}
			
			return (
				label.substring(0, endLength) +
				'...' +
				label.substring(label.length - endLength));
		}
		else
		{
			return label;
		}
	}
	
/*	this.shouldAddSearchResultsString = function()
	{
		if ( this.isSearchResult )
		{
			return this.searchResults > 1;
		}
		else
		{
			return this.searchResults > 0;
		}
	}
*/	
	this.sort = function()
	{
		this.children.sort(function(a, b){return b.getMagnitude() - a.getMagnitude()});
		
		for (var i = 0; i < this.children.length; i++)
		{
			this.children[i].sort();
		}
	}
}

var options;

function addOptionElement(position, innerHTML, title)
{
	var div = document.createElement("div");
//	div.style.position = 'absolute';
//	div.style.top = position + 'px';
	div.innerHTML = innerHTML;
//	div.style.display = 'block';
	div.style.padding = '2px';
	
	if ( title )
	{
		div.title = title;
	}
	
	options.appendChild(div);
	var height = 0;//div.clientHeight;
	return position + height;
}

function addOptionElements(hueName, hueDefault)
{
	options = document.createElement('div');
	options.style.position = 'absolute';
	options.style.top = '0px';
	options.addEventListener('mousedown', function(e) {mouseClick(e)}, false);
//	options.onmouseup = function(e) {mouseUp(e)}
	document.body.appendChild(options);
	
	document.body.style.font = '11px sans-serif';
	var position = 5;
	
	details = document.createElement('div');
	details.style.position = 'absolute';
	details.style.top = '1%';
	details.style.right = '2%';
	details.style.textAlign = 'right';
	document.body.insertBefore(details, canvas);
//		<div id="details" style="position:absolute;top:1%;right:2%;text-align:right;">

	details.innerHTML = '\
<span id="detailsName" style="font-weight:bold"></span>&nbsp;\
<input type="button" id="detailsExpand" onclick="expand(focusNode);"\
value="&harr;" title="Expand this wedge to become the new focus of the chart"/><br/>\
<div id="detailsInfo" style="float:right"></div>';

	keyControl = document.createElement('input');
	keyControl.type = 'button';
	keyControl.value = showKeys ? 'x' : '…';
	keyControl.style.position = '';
	keyControl.style.position = 'fixed';
	keyControl.style.visibility = 'hidden';
	
	document.body.insertBefore(keyControl, canvas);
	
	var logoElement = document.getElementById('logo');
	
	if ( logoElement )
	{
		logoImage = logoElement.src;
	}
	else
	{
		logoImage = 'http://marbl.github.io/Krona/img/logo-med.png';
	}
	
//	document.getElementById('options').style.fontSize = '9pt';
	position = addOptionElement
	(
		position,
'<a style="margin:2px" target="_blank" href="https://github.com/marbl/Krona/wiki"><img style="vertical-align:middle;width:108px;height:30px;" src="' + logoImage + '" alt="Logo of Krona"/></a><input type="button" id="back" value="&larr;" title="Go back (Shortcut: &larr;)"/>\
<input type="button" id="forward" value="&rarr;" title="Go forward (Shortcut: &rarr;)"/> \
&nbsp;Search: <input type="text" id="search"/>\
<input id="searchClear" type="button" value="x" onclick="clearSearch()"/> \
<span id="searchResults"></span>'
	);
	
	if ( datasets > 1 )
	{
		var size = datasets < datasetSelectSize ? datasets : datasetSelectSize;
		
		var select =
			'<table style="border-collapse:collapse;padding:0px"><tr><td style="padding:0px">' +
			'<select id="datasets" style="min-width:100px" size="' + size + '" onchange="onDatasetChange()">';
		
		for ( var i = 0; i < datasetNames.length; i++ )
		{
			select += '<option>' + datasetNames[i] + '</option>';
		}
		
		select +=
			'</select></td><td style="vertical-align:top;padding:1px;">' +
			'<input style="display:block" title="Previous dataset (Shortcut: &uarr;)" id="prevDataset" type="button" value="&uarr;" onclick="prevDataset()" disabled="true"/>' +
			'<input title="Next dataset (Shortcut: &darr;)" id="nextDataset" type="button" value="&darr;" onclick="nextDataset()"/><br/></td>' +
			'<td style="padding-top:1px;vertical-align:top"><input title="Switch to the last dataset that was viewed (Shortcut: TAB)" id="lastDataset" type="button" style="font:11px Times new roman" value="last" onclick="selectLastDataset()"/></td></tr></table>';
		
		position = addOptionElement(position + 5, select);
		
		datasetDropDown = document.getElementById('datasets');
		datasetButtonLast = document.getElementById('lastDataset');
		datasetButtonPrev = document.getElementById('prevDataset');
		datasetButtonNext = document.getElementById('nextDataset');
		
		position += datasetDropDown.clientHeight;
	}
	
	position = addOptionElement
	(
		position + 5,
'<input type="button" id="maxAbsoluteDepthDecrease" value="-"/>\
<span id="maxAbsoluteDepth"></span>\
&nbsp;<input type="button" id="maxAbsoluteDepthIncrease" value="+"/> Max depth',
'Maximum depth to display, counted from the top level \
and including collapsed wedges.'
	);
	
	position = addOptionElement
	(
		position,
'<input type="button" id="fontSizeDecrease" value="-"/>\
<span id="fontSize"></span>\
&nbsp;<input type="button" id="fontSizeIncrease" value="+"/> Font size'
	);
	
	position = addOptionElement
	(
		position,
'<input type="button" id="radiusDecrease" value="-"/>\
<input type="button" id="radiusIncrease" value="+"/> Chart size'
	);
	
	if ( hueName )
	{
		hueDisplayName = attributes[attributeIndex(hueName)].displayName;
		
		position = addOptionElement
		(
			position + 5,
			'<input type="checkbox" id="useHue" style="float:left" ' +
			'/><div>Color by<br/>' + hueDisplayName +
			'</div>'
		);
		
		useHueCheckBox = document.getElementById('useHue');
		useHueCheckBox.checked = hueDefault;
		useHueCheckBox.onclick = handleResize;
		useHueCheckBox.onmousedown = suppressEvent;
	}
	/*
	position = addOptionElement
	(
		position + 5,
		'&nbsp;<input type="checkbox" id="shorten" checked="checked" />Shorten labels</div>',
		'Prevent labels from overlapping by shortening them'
	);
	
	position = addOptionElement
	(
		position,
		'&nbsp;<input type="checkbox" id="compress" checked="checked" />Compress',
		'Compress wedges if needed to show the entire depth'
	);
	*/
	position = addOptionElement
	(
		position,
		'<input type="checkbox" id="showMagnitude" checked="checked" />Show magnitudes',
		'Show magnitudes in labels'
	);
	
	position = addOptionElement
	(
		position,
		'<input type="checkbox" id="collapse" checked="checked" />Collapse',
		'Collapse wedges that are redundant (entirely composed of another wedge)'
	);
	
	position = addOptionElement
	(
		position + 5,
		'<input type="button" id="snapshot" value="Snapshot"/>',
'Render the current view as SVG (Scalable Vector Graphics), a publication-\
quality format that can be printed and saved (see Help for browser compatibility)'
	);
	
	position = addOptionElement
	(
		position + 5,
'<input type="button" id="linkButton" value="Link"/>\
<input type="text" size="30" id="linkText"/>',
'Show a link to this view that can be copied for bookmarking or sharing'
	);
	
	position = addOptionElement
	(
		position + 5,
'<input type="button" id="help" value="?"\
onclick="window.open(\'https://github.com/marbl/Krona/wiki/Browsing%20Krona%20charts\', \'help\')"/>',
'Help'
	);
}

function arrow(angleStart, angleEnd, radiusInner)
{
	if ( context.globalAlpha == 0 )
	{
		return;
	}
	
	var angleCenter = (angleStart + angleEnd) / 2;
	var radiusArrowInner = radiusInner - gRadius / 10;//nodeRadius * gRadius;
	var radiusArrowOuter = gRadius * 1.1;//(1 + nodeRadius);
	var radiusArrowCenter = (radiusArrowInner + radiusArrowOuter) / 2;
	var pointLength = (radiusArrowOuter - radiusArrowInner) / 5;
	
	context.fillStyle = highlightFill;
	context.lineWidth = highlightLineWidth;
	
	// First, mask out the first half of the arrow.  This will prevent the tips
	// from superimposing if the arrow goes most of the way around the circle.
	// Masking is done by setting the clipping region to the inverse of the
	// half-arrow, which is defined by cutting the half-arrow out of a large
	// rectangle
	//
	context.beginPath();
	context.arc(0, 0, radiusInner, angleCenter, angleEnd, false);
	context.lineTo
	(
		radiusArrowInner * Math.cos(angleEnd),
		radiusArrowInner * Math.sin(angleEnd)
	);
	context.lineTo
	(
		radiusArrowCenter * Math.cos(angleEnd) - pointLength * Math.sin(angleEnd),
		radiusArrowCenter * Math.sin(angleEnd) + pointLength * Math.cos(angleEnd)
	);
	context.lineTo
	(
		radiusArrowOuter * Math.cos(angleEnd),
		radiusArrowOuter * Math.sin(angleEnd)
	);
	context.arc(0, 0, gRadius, angleEnd, angleCenter, true);
	context.closePath();
	context.moveTo(-imageWidth, -imageHeight);
	context.lineTo(imageWidth, -imageHeight);
	context.lineTo(imageWidth, imageHeight);
	context.lineTo(-imageWidth, imageHeight);
	context.closePath();
	context.save();
	context.clip();
	
	// Next, draw the other half-arrow with the first half masked out
	//
	context.beginPath();
	context.arc(0, 0, radiusInner, angleCenter, angleStart, true);
	context.lineTo
	(
		radiusArrowInner * Math.cos(angleStart),
		radiusArrowInner * Math.sin(angleStart)
	);
	context.lineTo
	(
		radiusArrowCenter * Math.cos(angleStart) + pointLength * Math.sin(angleStart),
		radiusArrowCenter * Math.sin(angleStart) - pointLength * Math.cos(angleStart)
	);
	context.lineTo
	(
		radiusArrowOuter * Math.cos(angleStart),
		radiusArrowOuter * Math.sin(angleStart)
	);
	context.arc(0, 0, gRadius, angleStart, angleCenter, false);
	context.fill();
	context.stroke();
	
	// Finally, remove the clipping region and draw the first half-arrow.  This
	// half is extended slightly to fill the seam.
	//
	context.restore();
	context.beginPath();
	context.arc(0, 0, radiusInner, angleCenter - 2 / (2 * Math.PI * radiusInner), angleEnd, false);
	context.lineTo
	(
		radiusArrowInner * Math.cos(angleEnd),
		radiusArrowInner * Math.sin(angleEnd)
	);
	context.lineTo
	(
		radiusArrowCenter * Math.cos(angleEnd) - pointLength * Math.sin(angleEnd),
		radiusArrowCenter * Math.sin(angleEnd) + pointLength * Math.cos(angleEnd)
	);
	context.lineTo
	(
		radiusArrowOuter * Math.cos(angleEnd),
		radiusArrowOuter * Math.sin(angleEnd)
	);
	context.arc(0, 0, gRadius, angleEnd, angleCenter - 2 / (2 * Math.PI * gRadius), true);
	context.fill();
	context.stroke();
}

function attributeIndex(aname)
{
	for ( var i = 0 ; i < attributes.length; i++ )
	{
		if ( aname == attributes[i].name )
		{
			return i;
		}
	}
	
	return null;
}

function checkHighlight()
{
	var lastHighlightedNode = highlightedNode;
	var lastHighlightingHidden = highlightingHidden;
	
	highlightedNode = selectedNode;
	resetKeyOffset();
	
	if ( progress == 1 )
	{
		selectedNode.checkHighlight();
		if ( selectedNode.getParent() )
		{
			selectedNode.getParent().checkHighlightCenter();
		}
		
		focusNode.checkHighlightMap();
	}
	
	if ( highlightedNode != selectedNode )
	{
		if ( highlightedNode == focusNode )
		{
//			canvas.style.display='none';
//			window.resizeBy(1,0);
//			canvas.style.cursor='ew-resize';
//			window.resizeBy(-1,0);
//			canvas.style.display='inline';
		}
		else
		{
//			canvas.style.cursor='pointer';
		}
	}
	else
	{
//		canvas.style.cursor='auto';
	}
	
	if
	(
		(
			true ||
			highlightedNode != lastHighlightedNode ||
			highlightingHidden != highlightingHiddenLast
		) &&
		progress == 1
	)
	{
		draw(); // TODO: handle in update()
	}
}

function checkSelectedCollapse()
{
	var newNode = selectedNode;
	
	while ( newNode.getCollapse() )
	{
		newNode = newNode.children[0];
	}
	
	if ( newNode.children.length == 0 && newNode.getParent() )
	{
		newNode = newNode.getParent();
	}
	
	if ( newNode != selectedNode )
	{
		selectNode(newNode);
	}
}

function clearSearch()
{
	if ( search.value != '' )
	{
		search.value = '';
		onSearchChange();
	}
}

function createSVG()
{
	svgNS = "http://www.w3.org/2000/svg";
	var SVG = {};
	SVG.xlinkns = "http://www.w3.org/1999/xlink";
	
	var newSVG = document.createElementNS(svgNS, "svg:svg");
	
	newSVG.setAttribute("id", "canvas");
	// How big is the canvas in pixels
	newSVG.setAttribute("width", '100%');
	newSVG.setAttribute("height", '100%');
	// Set the coordinates used by drawings in the canvas
//	newSVG.setAttribute("viewBox", "0 0 " + imageWidth + " " + imageHeight);
	// Define the XLink namespace that SVG uses
	newSVG.setAttributeNS
	(
		"http://www.w3.org/2000/xmlns/",
		"xmlns:xlink",
		SVG.xlinkns
	);
	
	return newSVG;
}

function degrees(radians)
{
	return radians * 180 / Math.PI;
}

function draw()
{
	tweenFrames++;
	//resize();
//	context.fillRect(0, 0, imageWidth, imageHeight);
	context.clearRect(0, 0, imageWidth, imageHeight);
	
	context.font = fontNormal;
	context.textBaseline = 'middle';
	
	//context.strokeStyle = 'rgba(0, 0, 0, 0.3)';
	context.translate(centerX, centerY);
	
	resetKeyOffset();
	
	head.draw(false, false); // draw pie slices
	head.draw(true, false); // draw labels
	
	var pathRoot = selectedNode;
	
	if ( focusNode != 0 && focusNode != selectedNode )
	{
		context.globalAlpha = 1;
		focusNode.drawHighlight(true);
		pathRoot = focusNode;
	}
	
	if
	(
		highlightedNode &&
		highlightedNode.getDepth() >= selectedNode.getDepth() &&
		highlightedNode != focusNode
	)
	{
		if
		(
			progress == 1 &&
			highlightedNode != selectedNode &&
			(
				highlightedNode != focusNode ||
				focusNode.children.length > 0
			)
		)
		{
			context.globalAlpha = 1;
			highlightedNode.drawHighlight(true);
		}
		
		//pathRoot = highlightedNode;
	}
	else if
	(
		progress == 1 &&
		highlightedNode.getDepth() < selectedNode.getDepth()
	)
	{
		context.globalAlpha = 1;
		highlightedNode.drawHighlightCenter();
	}
	
	if ( quickLook && false) // TEMP
	{
		context.globalAlpha = 1 - progress / 2;
		selectedNode.drawHighlight(true);
	}
	else if ( progress < 1 )//&& zoomOut() )
	{
		if ( !zoomOut)//() )
		{
			context.globalAlpha = selectedNode.alphaLine.current();
			selectedNode.drawHighlight(true);
		}
		else if ( selectedNodeLast )
		{
			context.globalAlpha = 1 - 4 * Math.pow(progress - .5, 2);
			selectedNodeLast.drawHighlight(false);
		}
	}
	
	drawDatasetName();
	
	//drawHistory();
	
	context.translate(-centerX, -centerY);
	context.globalAlpha = 1;
	
	mapRadius =
		(imageHeight / 2 - details.clientHeight - details.offsetTop) /
		(pathRoot.getDepth() - 1) * 3 / 4 / 2;
	
	if ( mapRadius > maxMapRadius )
	{
		mapRadius = maxMapRadius;
	}
	
	mapBuffer = mapRadius / 2;
	
	//context.font = fontNormal;
	pathRoot.drawMap(pathRoot);
	
	if ( hueDisplayName && useHue() )
	{
		drawLegend();
	}
}

function drawBubble(angle, radius, width, radial, flip)
{
	var height = fontSize * 2;
	var x;
	var y;
	
	width = width + fontSize;
	
	if ( radial )
	{
		y = -fontSize;
		
		if ( flip )
		{
			x = radius - width + fontSize / 2;
		}
		else
		{
			x = radius - fontSize / 2;
		}
	}
	else
	{
		x = -width / 2;
		y = -radius - fontSize;
	}
	
	if ( snapshotMode )
	{
		drawBubbleSVG(x + centerX, y + centerY, width, height, fontSize, angle);
	}
	else
	{
		drawBubbleCanvas(x, y, width, height, fontSize, angle);
	}
}

function drawBubbleCanvas(x, y, width, height, radius, rotation)
{
	context.strokeStyle = 'black';
	context.lineWidth = highlightLineWidth;
	context.fillStyle = 'rgba(255, 255, 255, .75)';
	context.rotate(rotation);
	roundedRectangle(x, y, width, fontSize * 2, fontSize);
	context.fill();
	context.stroke();
	context.rotate(-rotation);
}

function drawBubbleSVG(x, y, width, height, radius, rotation)
{
	svg +=
		'<rect x="' + x + '" y="' + y +
		'" width="' + width +
		'" height="' + height +
		'" rx="' + radius +
		'" ry="' + radius +
		'" fill="rgba(255, 255, 255, .75)' +
		'" class="highlight" ' +
		'transform="rotate(' +
		degrees(rotation) + ',' + centerX + ',' + centerY +
		')"/>';
}

function drawDatasetName()
{
	var alpha = datasetAlpha.current();
	
	if ( alpha > 0 )
	{
		var radius = gRadius * compressedRadii[0] / -2;
		
		if ( alpha > 1 )
		{
			alpha = 1;
		}
		
		context.globalAlpha = alpha;
		
		drawBubble(0, -radius, datasetWidths[currentDataset], false, false);
		drawText(datasetNames[currentDataset], 0, radius, 0, 'center', true);
	}
}

function drawHistory()
{
	var alpha = 1;
	context.textAlign = 'center';
	
	for ( var i = 0; i < nodeHistoryPosition && alpha > 0; i++ )
	{
		
		context.globalAlpha = alpha - historyAlphaDelta * tweenFactor;
		context.fillText
		(
			nodeHistory[nodeHistoryPosition - i - 1].name,
			0,
			(i + tweenFactor) * historySpacingFactor * fontSize - 1
		);
		
		if ( alpha > 0 )
		{
			alpha -= historyAlphaDelta;
		}
	}
	
	context.globalAlpha = 1;
}

function drawLegend()
{
	var left = imageWidth * .01;
	var width = imageHeight * .0265;
	var height = imageHeight * .15;
	var top = imageHeight - fontSize * 3.5 - height;
	var textLeft = left + width + fontSize / 2;
	
	context.fillStyle = 'black';
	context.textAlign = 'start';
	context.font = fontNormal;
//	context.fillText(valueStartText, textLeft, top + height);
//	context.fillText(valueEndText, textLeft, top);
	context.fillText(hueDisplayName, left, imageHeight - fontSize * 1.5);
	
	var gradient = context.createLinearGradient(0, top + height, 0, top);
	
	for ( var i = 0; i < hueStopPositions.length; i++ )
	{
		gradient.addColorStop(hueStopPositions[i], hueStopHsl[i]);
		
		var textY = top + (1 - hueStopPositions[i]) * height;
		
		if
		(
			i == 0 ||
			i == hueStopPositions.length - 1 ||
			textY > top + fontSize && textY < top + height - fontSize
		)
		{
			context.fillText(hueStopText[i], textLeft, textY);
		}
	}
	
	context.fillStyle = gradient;
	context.fillRect(left, top, width, height);
	context.lineWidth = thinLineWidth;
	context.strokeRect(left, top, width, height);
}

function drawLegendSVG()
{
	var left = imageWidth * .01;
	var width = imageHeight * .0265;
	var height = imageHeight * .15;
	var top = imageHeight - fontSize * 3.5 - height;
	var textLeft = left + width + fontSize / 2;

	var text = '';
	
	text += svgText(hueDisplayName, left, imageHeight - fontSize * 1.5);
	
	var svgtest = '<linearGradient id="gradient" x1="0%" y1="100%" x2="0%" y2="0%">';
	
	for ( var i = 0; i < hueStopPositions.length; i++ )
	{
		svgtest +=
			'<stop offset="' + round(hueStopPositions[i] * 100) +
			'%" style="stop-color:' + hueStopHsl[i] + '"/>';
		
		var textY = top + (1 - hueStopPositions[i]) * height;
		
		if
		(
			i == 0 ||
			i == hueStopPositions.length - 1 ||
			textY > top + fontSize && textY < top + height - fontSize
		)
		{
			text += svgText(hueStopText[i], textLeft, textY);
		}
	}
	
	svgtest += '</linearGradient>';
	//alert(svgtest);
	svg += svgtest;
	svg +=
		'<rect style="fill:url(#gradient)" x="' + left + '" y="' + top +
		'" width="' + width + '" height="' + height + '"/>';
	
	svg += text;
}

function drawSearchHighlights(label, bubbleX, bubbleY, rotation, center)
{
	var index = -1;
	var labelLength = label.length;
	
	bubbleX -= fontSize / 4;
	
	do
	{
		index = label.toLowerCase().indexOf(search.value.toLowerCase(), index + 1);
		
		if ( index != -1 && index < labelLength )
		{
			var dim = context.measureText(label.substr(0, index));
			var x = bubbleX + dim.width;
			
			dim = context.measureText(label.substr(index, search.value.length));
			
			var y = bubbleY - fontSize * 3 / 4;
			var width = dim.width + fontSize / 2;
			var height = fontSize * 3 / 2;
			var radius = fontSize / 2;
			
			if ( snapshotMode )
			{
				if ( center )
				{
					x += centerX;
					y += centerY;
				}
				
				svg +=
					'<rect x="' + x + '" y="' + y +
					'" width="' + width +
					'" height="' + height +
					'" rx="' + radius +
					'" ry="' + radius +
					'" class="searchHighlight' +
					'" transform="rotate(' +
					degrees(rotation) + ',' + centerX + ',' + centerY +
					')"/>';
			}
			else
			{
				context.fillStyle = 'rgb(255, 255, 100)';
				context.rotate(rotation);
				roundedRectangle(x, y, width, height, radius);
				context.fill();
				context.rotate(-rotation);
			}
		}
	}
	while ( index != -1 && index < labelLength );
}

function drawText(text, x, y, angle, anchor, bold, color)
{
	if ( color == undefined )
	{
		color = 'black';
	}
	
	if ( snapshotMode )
	{
		svg +=
			'<text x="' + (centerX + x) + '" y="' + (centerY + y) +
			'" text-anchor="' + anchor + '" style="font-color:' + color + ';font-weight:' + (bold ? 'bold' : 'normal') +
			'" transform="rotate(' + degrees(angle) + ',' + centerX + ',' + centerY + ')">' +
			text + '</text>';
	}
	else
	{
		context.fillStyle = color;
		context.textAlign = anchor;
		context.font = bold ? fontBold : fontNormal;
		context.rotate(angle);
		context.fillText(text, x, y);
		context.rotate(-angle);
	}
}

function drawTextPolar
(
	text,
	innerText,
	angle,
	radius,
	radial,
	bubble,
	bold, 
	searchResult,
	searchResults
)
{
	var anchor;
	var textX;
	var textY;
	var spacer;
	var totalText = text;
	var flip;
	
	if ( snapshotMode )
	{
		spacer = '&#160;&#160;&#160;';
	}
	else
	{
		spacer = '   ';
	}
	
	if ( radial )
	{
		flip = angle < 3 * Math.PI / 2;
		
		if ( flip )
		{
			angle -= Math.PI;
			radius = -radius;
			anchor = 'end';
			
			if ( innerText )
			{
				totalText = text + spacer + innerText;
			}
		}
		else
		{
			anchor = 'start';
			
			if ( innerText )
			{
				totalText = innerText + spacer + text;
			}
		}
		
		textX = radius;
		textY = 0;
	}
	else
	{
		flip = angle < Math.PI || angle > 2 * Math.PI;
		var label;
		
		anchor = snapshotMode ? 'middle' : 'center';
		
		if ( flip )
		{
			angle -= Math.PI;
			radius = -radius;
		}
		
		angle += Math.PI / 2;
		textX = 0;
		textY = -radius;
	}
	
	if ( bubble )
	{
		var textActual = totalText;
		
		if ( innerText && snapshotMode )
		{
			if ( flip )
			{
				textActual = text + '   ' + innerText;
			}
			else
			{
				textActual = innerText + '   ' + text;
			}
		}
		
		if ( searchResults )
		{
			textActual = textActual + searchResultString(searchResults);
		}
		
		var textWidth = measureText(textActual, bold);
		
		var x = textX;
		
		if ( anchor == 'end' )
		{
			x -= textWidth;
		}
		else if ( anchor != 'start' )
		{
			// centered
			x -= textWidth / 2;
		}
		
		drawBubble(angle, radius, textWidth, radial, flip);
		
		if ( searchResult )
		{
			drawSearchHighlights
			(
				textActual,
				x,
				textY,
				angle,
				true
			)
		}
	}
	
	if ( searchResults )
	{
		totalText = totalText + searchResultString(searchResults);
	}
	
	drawText(totalText, textX, textY, angle, anchor, bold);
	
	return flip;
}

function drawTick(start, length, angle)
{
	if ( snapshotMode )
	{
		svg +=
			'<line x1="' + (centerX + start) +
			'" y1="' + centerY +
			'" x2="' + (centerX + start + length) +
			'" y2="' + centerY +
			'" class="tick" transform="rotate(' +
			degrees(angle) + ',' + centerX + ',' + centerY +
			')"/>';
	}
	else
	{
		context.rotate(angle);
		context.beginPath();
		context.moveTo(start, 0);
		context.lineTo(start + length, 0);
		context.lineWidth = thinLineWidth * 2;
		context.stroke();
		context.rotate(-angle);
	}
}

function drawWedge
(
	angleStart,
	angleEnd,
	radiusInner,
	radiusOuter,
	color,
	patternAlpha,
	highlight
)
{
	if ( context.globalAlpha == 0 )
	{
		return;
	}
	
	if ( snapshotMode )
	{
		if ( angleEnd == angleStart + Math.PI * 2 )
		{
			// fudge to prevent overlap, which causes arc ambiguity
			//
			angleEnd -= .1 / gRadius;
		}
		
		var longArc = angleEnd - angleStart > Math.PI ? 1 : 0;
		
		var x1 = centerX + radiusInner * Math.cos(angleStart);
		var y1 = centerY + radiusInner * Math.sin(angleStart);
		
		var x2 = centerX + gRadius * Math.cos(angleStart);
		var y2 = centerY + gRadius * Math.sin(angleStart);
		
		var x3 = centerX + gRadius * Math.cos(angleEnd);
		var y3 = centerY + gRadius * Math.sin(angleEnd);
		
		var x4 = centerX + radiusInner * Math.cos(angleEnd);
		var y4 = centerY + radiusInner * Math.sin(angleEnd);
		
		var dArray =
		[
			" M ", x1, ",", y1,
			" L ", x2, ",", y2,
			" A ", gRadius, ",", gRadius, " 0 ", longArc, ",1 ", x3, ",", y3,
			" L ", x4, ",", y4,
			" A ", radiusInner, ",", radiusInner, " 0 ", longArc, " 0 ", x1, ",", y1,
			" Z "
		];
		
		svg +=
			'<path class="'+ (highlight ? 'highlight' : 'wedge') + '" fill="' + color +
			'" d="' + dArray.join('') + '"/>';
		
		if ( patternAlpha > 0 )
		{
			svg +=
				'<path class="wedge" fill="url(#hiddenPattern)" d="' +
				dArray.join('') + '"/>';
		}
	}
	else
	{
		// fudge to prevent seams during animation
		//
		angleEnd += 1 / gRadius;
		
		context.fillStyle = color;
		context.beginPath();
		context.arc(0, 0, radiusInner, angleStart, angleEnd, false);
		context.arc(0, 0, radiusOuter, angleEnd, angleStart, true);
		context.closePath();
		context.fill();
		
		if ( patternAlpha > 0 )
		{
			context.save();
			context.clip();
			context.globalAlpha = patternAlpha;
			context.fillStyle = hiddenPattern;
			context.fill();
			context.restore();
		}
		
		if ( highlight )
		{
			context.lineWidth = highlight ? highlightLineWidth : thinLineWidth;
			context.strokeStyle = 'black';
			context.stroke();
		}
	}
}

function expand(node)
{
	selectNode(node);
	updateView();
}

function focusLost()
{
	mouseX = -1;
	mouseY = -1;
	checkHighlight();
	document.body.style.cursor = 'auto';
}

function fontSizeDecrease()
{
	if ( fontSize > 1 )
	{
		fontSize--;
		updateViewNeeded = true;
	}
}

function fontSizeIncrease()
{
	fontSize++;
	updateViewNeeded = true;
}

function getGetString(name, value, bool)
{
	return name + '=' + (bool ? value ? 'true' : 'false' : value);
}

function hideLink()
{
	hide(linkText);
	show(linkButton);
}

function show(object)
{
	object.style.display = 'inline';
}

function hide(object)
{
	object.style.display = 'none';
}

function showLink()
{
	var urlHalves = String(document.location).split('?');
	var newGetVariables = new Array();
	
	newGetVariables.push
	(
		getGetString('dataset', currentDataset, false),
		getGetString('node', selectedNode.id, false),
		getGetString('collapse', collapse, true),
		getGetString('showMagnitude', showMagnitude, true),
		getGetString('color', useHue(), true),
		getGetString('depth', maxAbsoluteDepth - 1, false),
		getGetString('font', fontSize, false),
		getGetString('key', showKeys, true)
	);
	
	hide(linkButton);
	show(linkText);
	linkText.value = urlHalves[0] + '?' + getVariables.concat(newGetVariables).join('&');
	//linkText.disabled = false;
	linkText.focus();
	linkText.select();
	//linkText.disabled = true;
//	document.location = urlHalves[0] + '?' + getVariables.join('&');
}

function getFirstChild(element)
{
	element = element.firstChild;
	
	if ( element && element.nodeType != 1 )
	{
		element = getNextSibling(element);
	}
	
	return element;
}

function getNextSibling(element)
{
	do
	{
		element = element.nextSibling;
	}
	while ( element && element.nodeType != 1 );
	
	return element;
}

function getPercentage(fraction)
{
	return round(fraction * 100);
}

function hslText(hue)
{
	if ( 1 || snapshotMode )
	{
		// Safari doesn't seem to allow hsl() in SVG
		
		var rgb = hslToRgb(hue, saturation, (lightnessBase + lightnessMax) / 2);
		
		return rgbText(rgb.r, rgb.g, rgb.b);
	}
	else
	{
		var hslArray =
		[
			'hsl(',
			Math.floor(hue * 360),
			',',
			Math.floor(saturation * 100),
			'%,',
			Math.floor((lightnessBase + lightnessMax) * 50),
			'%)'
		];
		
		return hslArray.join('');
	}
}

function hslToRgb(h, s, l)
{
	var m1, m2;
	var r, g, b;
	
	if (s == 0)
	{
		r = g = b = Math.floor((l * 255));
	}
	else
	{
		if (l <= 0.5)
		{
			m2 = l * (s + 1);
		}
		else
		{
			m2 = l + s - l * s;
		}
		
		m1 = l * 2 - m2;
		
		r = Math.floor(hueToRgb(m1, m2, h + 1 / 3));
		g = Math.floor(hueToRgb(m1, m2, h));
		b = Math.floor(hueToRgb(m1, m2, h - 1/3));
	}
	
	return {r: r, g: g, b: b};
}

function hueToRgb(m1, m2, hue)
{
	var v;
	
	while (hue < 0)
	{
		hue += 1;
	}
	
	while (hue > 1)
	{
		hue -= 1;
	}
	
	if (6 * hue < 1)
		v = m1 + (m2 - m1) * hue * 6;
	else if (2 * hue < 1)
		v = m2;
	else if (3 * hue < 2)
		v = m1 + (m2 - m1) * (2/3 - hue) * 6;
	else
		v = m1;

	return 255 * v;
}

function interpolateHue(hueStart, hueEnd, valueStart, valueEnd)
{
	// since the gradient will be RGB based, we need to add stops to hit all the
	// colors in the hue spectrum
	
	hueStopPositions = new Array();
	hueStopHsl = new Array();
	hueStopText = new Array();
	
	hueStopPositions.push(0);
	hueStopHsl.push(hslText(hueStart));
	hueStopText.push(round(valueStart));
	
	for
	(
		var i = (hueStart > hueEnd ? 5 / 6 : 1 / 6);
		(hueStart > hueEnd ? i > 0 : i < 1);
		i += (hueStart > hueEnd ? -1 : 1) / 6
	)
	{
		if
		(
			hueStart > hueEnd ?
				i > hueEnd && i < hueStart :
				i > hueStart && i < hueEnd
		)
		{
			hueStopPositions.push(lerp(i, hueStart, hueEnd, 0, 1));
			hueStopHsl.push(hslText(i));
			hueStopText.push(round(lerp
			(
				i,
				hueStart,
				hueEnd,
				valueStart,
				valueEnd
			)));
		}
	}
	
	hueStopPositions.push(1);
	hueStopHsl.push(hslText(hueEnd));
	hueStopText.push(round(valueEnd));
}

function keyLineAngle(angle, keyAngle, bendRadius, keyX, keyY, pointsX, pointsY)
{
	if ( angle < Math.PI / 2 && keyY < bendRadius * Math.sin(angle) 
	|| angle > Math.PI / 2 && keyY < bendRadius)
	{
		return Math.asin(keyY / bendRadius);
	}
	else
	{
		// find the angle of the normal to a tangent line that goes to
		// the label
		
		var textDist = Math.sqrt
		(
			Math.pow(keyX, 2) +
			Math.pow(keyY, 2)
		);
		
		var tanAngle = Math.acos(bendRadius / textDist) + keyAngle;
		
		if ( angle < tanAngle || angle < Math.PI / 2 )//|| labelLeft < centerX )
		{
			// angle doesn't reach far enough for tangent; collapse and
			// connect directly to label
			
			if ( keyY / Math.tan(angle) > 0 )
			{
				pointsX.push(keyY / Math.tan(angle));
				pointsY.push(keyY);
			}
			else
			{
				pointsX.push(bendRadius * Math.cos(angle));
				pointsY.push(bendRadius * Math.sin(angle));
			}
			
			return angle;
		}
		else
		{
			return tanAngle;
		}
	}
}

function keyOffset()
{
	return imageHeight - (keys - currentKey + 1) * (keySize + keyBuffer) + keyBuffer - margin;
}

function lerp(value, fromStart, fromEnd, toStart, toEnd)
{
	return (value - fromStart) *
		(toEnd - toStart) /
		(fromEnd - fromStart) +
		toStart;
}

function createCanvas()
{
	canvas = document.createElement('canvas');
	document.body.appendChild(canvas);
	context = canvas.getContext('2d');
}

function load()
{
	document.body.style.overflow = "hidden";
	document.body.style.margin = 0;
	
	createCanvas();
	
	if ( context == undefined )
	{
		document.body.innerHTML = '\
<br/>This browser does not support HTML5 (see \
<a href="https://github.com/marbl/Krona/wiki/Browser%20support">Browser support</a>).\
	';
		return;
	}

	if ( typeof context.fillText != 'function' )
	{
		document.body.innerHTML = '\
<br/>This browser does not support HTML5 canvas text (see \
<a href="https://github.com/marbl/Krona/wiki/Browser%20support">Browser support</a>).\
	';
		return;
	}
	
	resize();
	
	var kronaElement = document.getElementsByTagName('krona')[0];
	
	var magnitudeName;
	var hueName;
	var hueDefault;
	var hueStart;
	var hueEnd;
	var valueStart;
	var valueEnd;
	
	if ( kronaElement.getAttribute('collapse') != undefined )
	{
		collapse = kronaElement.getAttribute('collapse') == 'true';
	}
	
	if ( kronaElement.getAttribute('key') != undefined )
	{
		showKeys = kronaElement.getAttribute('key') == 'true';
	}
	
	for
	(
		var element = getFirstChild(kronaElement);
		element;
		element = getNextSibling(element)
	)
	{
		switch ( element.tagName.toLowerCase() )
		{
			case 'attributes':
				magnitudeName = element.getAttribute('magnitude');
				//
				for
				(
					var attributeElement = getFirstChild(element);
					attributeElement;
					attributeElement = getNextSibling(attributeElement)
				)
				{
					var tag = attributeElement.tagName.toLowerCase();
					
					if ( tag == 'attribute' )
					{
						var attribute = new Attribute();
						attribute.name = attributeElement.firstChild.nodeValue.toLowerCase();
						attribute.displayName = attributeElement.getAttribute('display');
						
						if ( attributeElement.getAttribute('hrefBase') )
						{
							attribute.hrefBase = attributeElement.getAttribute('hrefBase');
						}
						
						if ( attributeElement.getAttribute('target') )
						{
							attribute.target = attributeElement.getAttribute('target');
						}
						
						if ( attribute.name == magnitudeName )
						{
							magnitudeIndex = attributes.length;
						}
						
						if ( attributeElement.getAttribute('listAll') )
						{
							attribute.listAll = attributeElement.getAttribute('listAll').toLowerCase();
						}
						else if ( attributeElement.getAttribute('listNode') )
						{
							attribute.listNode = attributeElement.getAttribute('listNode').toLowerCase();
						}
						else if ( attributeElement.getAttribute('dataAll') )
						{
							attribute.dataAll = attributeElement.getAttribute('dataAll').toLowerCase();
						}
						else if ( attributeElement.getAttribute('dataNode') )
						{
							attribute.dataNode = attributeElement.getAttribute('dataNode').toLowerCase();
						}
						
						if ( attributeElement.getAttribute('postUrl') )
						{
							attribute.postUrl = attributeElement.getAttribute('postUrl');
						}
						
						if ( attributeElement.getAttribute('postVar') )
						{
							attribute.postVar = attributeElement.getAttribute('postVar');
						}
						
						if ( attributeElement.getAttribute('mono') )
						{
							attribute.mono = true;
						}
						
						attributes.push(attribute);
					}
					else if ( tag == 'list' )
					{
						var attribute = new Attribute();
						
						attribute.name = attributeElement.firstChild.nodeValue;
						attribute.list = true;
						attributes.push(attribute);
					}
					else if ( tag == 'data' )
					{
						var attribute = new Attribute();
						
						attribute.name = attributeElement.firstChild.nodeValue;
						attribute.data = true;
						attributes.push(attribute);
						
						var enableScript = document.createElement('script');
						var date = new Date();
						enableScript.src =
							attributeElement.getAttribute('enable') + '?' +
							date.getTime();
						document.body.appendChild(enableScript);
					}
				}
				break;
			
			case 'color':
				hueName = element.getAttribute('attribute');
				hueStart = Number(element.getAttribute('hueStart')) / 360;
				hueEnd = Number(element.getAttribute('hueEnd')) / 360;
				valueStart = Number(element.getAttribute('valueStart'));
				valueEnd = Number(element.getAttribute('valueEnd'));
				//
				interpolateHue(hueStart, hueEnd, valueStart, valueEnd);
				//
				if ( element.getAttribute('default') == 'true' )
				{
					hueDefault = true;
				}
				break;
			
			case 'datasets':
				datasetNames = new Array();
				//
				for ( j = getFirstChild(element); j; j = getNextSibling(j) )
				{
					datasetNames.push(j.firstChild.nodeValue);
				}
				datasets = datasetNames.length;
				break;
			
			case 'node':
				head = loadTreeDOM
				(
					element,
					magnitudeName,
					hueName,
					hueStart,
					hueEnd,
					valueStart,
					valueEnd
				);
				break;
		}
	}
	
	// get GET options
	//
	var urlHalves = String(document.location).split('?');
	var datasetDefault = 0;
	var maxDepthDefault;
	var nodeDefault = 0;
	//
	if ( urlHalves[1] )
	{
		var vars = urlHalves[1].split('&');
		
		for ( i = 0; i < vars.length; i++ )
		{
			var pair = vars[i].split('=');
			
			switch ( pair[0] )
			{
				case 'collapse':
					collapse = pair[1] == 'true';
					break;
				
				case 'showMagnitude':
					showMagnitude = pair[1] == 'true';
					break;
				
				case 'color':
					hueDefault = pair[1] == 'true';
					break;
				
				case 'dataset':
					datasetDefault = Number(pair[1]);
					break;
					
				case 'depth':
					maxDepthDefault = Number(pair[1]) + 1;
					break;
				
				case 'key':
					showKeys = pair[1] == 'true';
					break;
				
				case 'font':
					fontSize = Number(pair[1]);
					break;
				
				case 'node':
					nodeDefault = Number(pair[1]);
					break;
				
				default:
					getVariables.push(pair[0] + '=' + pair[1]);
					break;
			}
		}
	}
	
	addOptionElements(hueName, hueDefault);
	setCallBacks();
	
	head.sort();
	maxAbsoluteDepth = 0;
	selectDataset(datasetDefault);
	
	if ( maxDepthDefault && maxDepthDefault < head.maxDepth )
	{
		maxAbsoluteDepth = maxDepthDefault;
	}
	else
	{
		maxAbsoluteDepth = head.maxDepth;
	}
	
	selectNode(nodes[nodeDefault]);
	
	setInterval(update, 20);
	
	window.onresize = handleResize;
	updateMaxAbsoluteDepth();
	updateViewNeeded = true;
}

function loadTreeDOM
(
	domNode,
	magnitudeName,
	hueName,
	hueStart,
	hueEnd,
	valueStart,
	valueEnd
)
{
	var newNode = new Node();
	
	newNode.name = domNode.getAttribute('name');
	
	if ( domNode.getAttribute('href') )
	{
		newNode.href = domNode.getAttribute('href');
	}
	
	if ( hueName )
	{
		newNode.hues = new Array();
	}
	
	for ( var i = getFirstChild(domNode); i; i = getNextSibling(i) )
	{
		switch ( i.tagName.toLowerCase() )
		{
		case 'node': 
			var newChild = loadTreeDOM
			(
				i,
				magnitudeName,
				hueName,
				hueStart,
				hueEnd,
				valueStart,
				valueEnd
			);
			newChild.parent = newNode;
			newNode.children.push(newChild);
			break;
			
		default:
			var attributeName = i.tagName.toLowerCase();
			var index = attributeIndex(attributeName);
			//
			newNode.attributes[index] = new Array();
			//
			for ( var j = getFirstChild(i); j; j = getNextSibling(j) )
			{
				if ( attributes[index] == undefined )
				{
					var x = 5;
				}
				if ( attributes[index].list )
				{
					newNode.attributes[index].push(new Array());
					
					for ( var k = getFirstChild(j); k; k = getNextSibling(k) )
					{
						newNode.attributes[index][newNode.attributes[index].length - 1].push(k.firstChild.nodeValue);
					}
				}
				else
				{
					var value = j.firstChild ? j.firstChild.nodeValue : '';
					
					if ( j.getAttribute('href') )
					{
						var target;
						
						if ( attributes[index].target )
						{
							target = ' target="' + attributes[index].target + '"';
						}
						
						value = '<a href="' + attributes[index].hrefBase + j.getAttribute('href') + '"' + target + '>' + value + '</a>';
					}
					
					newNode.attributes[index].push(value);
				}
			}
			//
			if ( attributeName == magnitudeName || attributeName == hueName )
			{
				for ( j = 0; j < datasets; j++ )
				{
					var value = newNode.attributes[index][j] == undefined ? 0 : Number(newNode.attributes[index][j]);
					
					newNode.attributes[index][j] = value;
					
					if ( attributeName == hueName )
					{
						var hue = lerp
						(
							value,
							valueStart,
							valueEnd,
							hueStart,
							hueEnd
						);
						
						if ( hue < hueStart == hueStart < hueEnd )
						{
							hue = hueStart;
						}
						else if ( hue > hueEnd == hueStart < hueEnd )
						{
							hue = hueEnd;
						}
						
						newNode.hues[j] = hue;
					}
				}
				
				if ( attributeName == hueName )
				{
					newNode.hue = new Tween(newNode.hues[0], newNode.hues[0]);
				}
			}
			break;
		}
	}
	
	return newNode;
}

function maxAbsoluteDepthDecrease()
{
	if ( maxAbsoluteDepth > 2 )
	{
		maxAbsoluteDepth--;
		head.setMaxDepths();
		handleResize();
	}
}

function maxAbsoluteDepthIncrease()
{
	if ( maxAbsoluteDepth < head.maxDepth )
	{
		maxAbsoluteDepth++;
		head.setMaxDepths();
		handleResize();
	}
}

function measureText(text, bold)
{
	context.font = bold ? fontBold : fontNormal;
	var dim = context.measureText(text);
	return dim.width;
}

function min(a, b)
{
	return a < b ? a : b;
}

function minWidth()
{
	// Min wedge width (at center) for displaying a node (or for displaying a
	// label if it's at the highest level being viewed, multiplied by 2 to make
	// further calculations simpler
	
	return (fontSize * 2.3);
}

function mouseMove(e)
{
	mouseX = e.pageX;
	mouseY = e.pageY - headerHeight;
	mouseXRel = (mouseX - centerX) * backingScale()
	mouseYRel = (mouseY - centerY) * backingScale()
	
	if ( head && ! quickLook )
	{
		checkHighlight();
	}
}

function mouseClick(e)
{
	if ( highlightedNode == focusNode && focusNode != selectedNode || selectedNode.hasParent(highlightedNode) )
	{
		if ( highlightedNode.hasChildren() )
		{
			expand(highlightedNode);
		}
	}
	else if ( progress == 1 )//( highlightedNode != selectedNode )
	{
		setFocus(highlightedNode);
//		document.body.style.cursor='ew-resize';
		draw();
		checkHighlight();
		var date = new Date();
		mouseDownTime = date.getTime();
		mouseDown = true;
	}
}

function mouseUp(e)
{
	if ( quickLook )
	{
		navigateBack();
		quickLook = false;
	}
	
	mouseDown = false;
}

function navigateBack()
{
	if ( nodeHistoryPosition > 0 )
	{
		nodeHistory[nodeHistoryPosition] = selectedNode;
		nodeHistoryPosition--;
		
		if ( nodeHistory[nodeHistoryPosition].collapse )
		{
			collapseCheckBox.checked = collapse = false;
		}
		
		setSelectedNode(nodeHistory[nodeHistoryPosition]);
		updateDatasetButtons();
		updateView();
	}
}

function navigateUp()
{
	if ( selectedNode.getParent() )
	{
		selectNode(selectedNode.getParent());
		updateView();
	}
}

function navigateForward()
{
	if ( nodeHistoryPosition < nodeHistory.length - 1 )
	{
		nodeHistoryPosition++;
		var newNode = nodeHistory[nodeHistoryPosition];
		
		if ( newNode.collapse )
		{
			collapseCheckBox.checked = collapse = false;
		}
		
		if ( nodeHistoryPosition == nodeHistory.length - 1 )
		{
			// this will ensure the forward button is disabled
			
			nodeHistory.length = nodeHistoryPosition;
		}
		
		setSelectedNode(newNode);
		updateDatasetButtons();
		updateView();
	}
}

function nextDataset()
{
	var newDataset = currentDataset;
	
	do
	{
		if ( newDataset == datasets - 1 )
		{
			newDataset = 0;
		}
		else
		{
			newDataset++;
		}
	}
	while ( datasetDropDown.options[newDataset].disabled )
	
	selectDataset(newDataset);
}

function onDatasetChange()
{
	selectDataset(datasetDropDown.selectedIndex);
}

function onKeyDown(event)
{
	if
	(
		event.keyCode == 37 &&
		document.activeElement.id != 'search' &&
		document.activeElement.id != 'linkText'
	)
	{
		navigateBack();
		event.preventDefault();
	}
	else if
	(
		event.keyCode == 39 &&
		document.activeElement.id != 'search' &&
		document.activeElement.id != 'linkText'
	)
	{
		navigateForward();
		event.preventDefault();
	}
	else if ( event.keyCode == 38 && datasets > 1 )
	{
		prevDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
	else if ( event.keyCode == 40 && datasets > 1 )
	{
		nextDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
	else if ( event.keyCode == 9 && datasets > 1 )
	{
		selectLastDataset();
		event.preventDefault();
	}
	else if ( event.keyCode == 83 )
	{
		progress += .2;
	}
	else if ( event.keyCode == 66 )
	{
		progress -= .2;
	}
	else if ( event.keyCode == 70 )
	{
		progress = 1;
	}
}

function onKeyPress(event)
{
	if ( event.keyCode == 38 && datasets > 1 )
	{
//		prevDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
	else if ( event.keyCode == 40 && datasets > 1 )
	{
//		nextDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
}

function onKeyUp(event)
{
	if ( event.keyCode == 27 && document.activeElement.id == 'search' )
	{
		search.value = '';
		onSearchChange();
	}
	else if ( event.keyCode == 38 && datasets > 1 )
	{
//		prevDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
	else if ( event.keyCode == 40 && datasets > 1 )
	{
//		nextDataset();
		
		//if ( document.activeElement.id == 'datasets' )
		{
			event.preventDefault();
		}
	}
}

function onSearchChange()
{
	nSearchResults = 0;
	head.search();
	
	if ( search.value == '' )
	{
		searchResults.innerHTML = '';
	}
	else
	{
		searchResults.innerHTML = nSearchResults + ' results';
	}
	
	setFocus(selectedNode);
	draw();
}

function post(url, variable, value, postWindow)
{
	var form = document.createElement('form');
	var input = document.createElement('input');
	var inputDataset = document.createElement('input');
	
	form.appendChild(input);
	form.appendChild(inputDataset);
	
	form.method = "POST";
	form.action = url;
	
	if ( postWindow == undefined )
	{
		form.target = '_blank';
		postWindow = window;
	}
	
	input.type = 'hidden';
	input.name = variable;
	input.value = value;
	
	inputDataset.type = 'hidden';
	inputDataset.name = 'dataset';
	inputDataset.value = currentDataset;
	
	postWindow.document.body.appendChild(form);
	form.submit();
}

function prevDataset()
{
	var newDataset = currentDataset;
	
	do
	{
		if ( newDataset == 0 )
		{
			newDataset = datasets - 1;
		}
		else
		{
			newDataset--;
		}
	}
	while ( datasetDropDown.options[newDataset].disabled );
	
	selectDataset(newDataset);
}

function radiusDecrease()
{
	if ( bufferFactor < .309 )
	{
		bufferFactor += .03;
		updateViewNeeded = true;
	}
}

function radiusIncrease()
{
	if ( bufferFactor > .041 )
	{
		bufferFactor -= .03;
		updateViewNeeded = true;
	}
}

function resetKeyOffset()
{
	currentKey = 1;
	keyMinTextLeft = centerX + gRadius + buffer - buffer / (keys + 1) / 2 + fontSize / 2;
	keyMinAngle = 0;
}

function rgbText(r, g, b)
{
	var rgbArray =
	[
		"rgb(",
		Math.floor(r),
		",",
		Math.floor(g),
		",",
		Math.floor(b),
		")"
	];
	
	return rgbArray.join('');
}

function round(number)
{
	if ( number >= 1 || number <= -1 )
	{
		return number.toFixed(0);
	}
	else
	{
		return number.toPrecision(1);
	}
}

function roundedRectangle(x, y, width, height, radius)
{
	if ( radius * 2 > width )
	{
		radius = width / 2;
	}
	
	if ( radius * 2 > height )
	{
		radius = height / 2;
	}
	
	context.beginPath();
	context.arc(x + radius, y + radius, radius, Math.PI, Math.PI * 3 / 2, false);
	context.lineTo(x + width - radius, y);
	context.arc(x + width - radius, y + radius, radius, Math.PI * 3 / 2, Math.PI * 2, false);
	context.lineTo(x + width, y + height - radius);
	context.arc(x + width - radius, y + height - radius, radius, 0, Math.PI / 2, false);
	context.lineTo(x + radius, y + height);
	context.arc(x + radius, y + height - radius, radius, Math.PI / 2, Math.PI, false);
	context.lineTo(x, y + radius);
}

function passClick(e)
{
	mouseClick(e);
}

function searchResultString(results)
{
	var searchResults = this.searchResults;
	
	if ( this.isSearchResult )
	{
		// don't count ourselves
		searchResults--;
	}
	
	return ' - ' + results + (results > 1 ? ' results' : ' result');
}

function setCallBacks()
{
	canvas.onselectstart = function(){return false;} // prevent unwanted highlighting
	options.onselectstart = function(){return false;} // prevent unwanted highlighting
	document.onmousemove = mouseMove;
	window.onblur = focusLost;
	window.onmouseout = focusLost;
	document.onkeyup = onKeyUp;
	document.onkeydown = onKeyDown;
	canvas.onmousedown = mouseClick;
	document.onmouseup = mouseUp;
	keyControl.onclick = toggleKeys;
	showMagnitudeCheckBox = document.getElementById('showMagnitude');
	showMagnitudeCheckBox.checked = showMagnitude;
	showMagnitudeCheckBox.onclick = handleResize;
	collapseCheckBox = document.getElementById('collapse');
	collapseCheckBox.checked = collapse;
	collapseCheckBox.onclick = handleResize;
	collapseCheckBox.onmousedown = suppressEvent;
	maxAbsoluteDepthText = document.getElementById('maxAbsoluteDepth');
	maxAbsoluteDepthButtonDecrease = document.getElementById('maxAbsoluteDepthDecrease');
	maxAbsoluteDepthButtonIncrease = document.getElementById('maxAbsoluteDepthIncrease');
	maxAbsoluteDepthButtonDecrease.onclick = maxAbsoluteDepthDecrease;
	maxAbsoluteDepthButtonIncrease.onclick = maxAbsoluteDepthIncrease;
	maxAbsoluteDepthButtonDecrease.onmousedown = suppressEvent;
	maxAbsoluteDepthButtonIncrease.onmousedown = suppressEvent;
	fontSizeText = document.getElementById('fontSize');
	fontSizeButtonDecrease = document.getElementById('fontSizeDecrease');
	fontSizeButtonIncrease = document.getElementById('fontSizeIncrease');
	fontSizeButtonDecrease.onclick = fontSizeDecrease;
	fontSizeButtonIncrease.onclick = fontSizeIncrease;
	fontSizeButtonDecrease.onmousedown = suppressEvent;
	fontSizeButtonIncrease.onmousedown = suppressEvent;
	radiusButtonDecrease = document.getElementById('radiusDecrease');
	radiusButtonIncrease = document.getElementById('radiusIncrease');
	radiusButtonDecrease.onclick = radiusDecrease;
	radiusButtonIncrease.onclick = radiusIncrease;
	radiusButtonDecrease.onmousedown = suppressEvent;
	radiusButtonIncrease.onmousedown = suppressEvent;
	maxAbsoluteDepth = 0;
	backButton = document.getElementById('back');
	backButton.onclick = navigateBack;
	backButton.onmousedown = suppressEvent;
	forwardButton = document.getElementById('forward');
	forwardButton.onclick = navigateForward;
	forwardButton.onmousedown = suppressEvent;
	snapshotButton = document.getElementById('snapshot');
	snapshotButton.onclick = snapshot;
	snapshotButton.onmousedown = suppressEvent;
	detailsName = document.getElementById('detailsName');
	detailsExpand = document.getElementById('detailsExpand');
	detailsInfo = document.getElementById('detailsInfo');
	search = document.getElementById('search');
	search.onkeyup = onSearchChange;
	search.onmousedown = suppressEvent;
	searchResults = document.getElementById('searchResults');
	useHueDiv = document.getElementById('useHueDiv');
	linkButton = document.getElementById('linkButton');
	linkButton.onclick = showLink;
	linkButton.onmousedown = suppressEvent;
	linkText = document.getElementById('linkText');
	linkText.onblur = hideLink;
	linkText.onmousedown = suppressEvent;
	hide(linkText);
	var helpButton = document.getElementById('help');
	helpButton.onmousedown = suppressEvent;
	var searchClear = document.getElementById('searchClear');
	searchClear.onmousedown = suppressEvent;
	if ( datasets > 1 )
	{
		datasetDropDown.onmousedown = suppressEvent;
		var prevDatasetButton = document.getElementById('prevDataset');
		prevDatasetButton.onmousedown = suppressEvent;
		var nextDatasetButton = document.getElementById('nextDataset');
		nextDatasetButton.onmousedown = suppressEvent;
		var lastDatasetButton = document.getElementById('lastDataset');
		lastDatasetButton.onmousedown = suppressEvent;
	}
	
	image = document.getElementById('hiddenImage');
	
	if ( image.complete )
	{
		hiddenPattern = context.createPattern(image, 'repeat');
	}
	else
	{
		image.onload = function()
		{
			hiddenPattern = context.createPattern(image, 'repeat');
		}
	}
	
	var loadingImageElement = document.getElementById('loadingImage');
	
	if ( loadingImageElement )
	{
		loadingImage = loadingImageElement.src;
	}
}

function selectDataset(newDataset)
{
	lastDataset = currentDataset;
	currentDataset = newDataset
	if ( datasets > 1 )
	{
		datasetDropDown.selectedIndex = currentDataset;
		updateDatasetButtons();
		datasetAlpha.start = 1.5;
		datasetChanged = true;
	}
	head.setMagnitudes(0);
	head.setDepth(1, 1);
	head.setMaxDepths();
	handleResize();
}

function selectLastDataset()
{
	selectDataset(lastDataset);
	handleResize();
}

function selectNode(newNode)
{
	if ( selectedNode != newNode )
	{
		// truncate history at current location to create a new branch
		//
		nodeHistory.length = nodeHistoryPosition;
		
		if ( selectedNode != 0 )
		{
			nodeHistory.push(selectedNode);
			nodeHistoryPosition++;
		}
		
		setSelectedNode(newNode);
		//updateView();
	}
	
	updateDatasetButtons();
}

function setFocus(node)
{
	if ( node == focusNode )
	{
//		return;
	}
	
	focusNode = node;
	
	if ( node.href )
	{
		detailsName.innerHTML =
			'<a target="_blank" href="' + node.href + '">' + node.name + '</a>';
	}
	else
	{
		detailsName.innerHTML = node.name;
	}
	
	var table = '<table>';
	//TODO: use CSS margins instead of an additional column
	table += '<tr><td></td><td></td></tr>';
	
	for ( var i = 0; i < node.attributes.length; i++ )
	{
		if ( attributes[i].displayName && node.attributes[i] != undefined )
		{
			var index = node.attributes[i].length == 1 && attributes[i].mono ? 0 : currentDataset;
			
			if ( typeof node.attributes[i][currentDataset] == 'number' || node.attributes[i][index] != undefined && node.attributes[i][currentDataset] != '' )
			{
				var value = node.attributes[i][index];
				
				if ( attributes[i].listNode != undefined )
				{
					value =
						'<a href="" onclick="showList(' +
						attributeIndex(attributes[i].listNode) + ',' + i +
						',false);return false;" title="Show list">' +
						value + '</a>';
				}
				else if ( attributes[i].listAll != undefined )
				{
					value =
						'<a href="" onclick="showList(' +
						attributeIndex(attributes[i].listAll) + ',' + i +
						',true);return false;" title="Show list">' +
						value + '</a>';
				}
				else if ( attributes[i].dataNode != undefined && dataEnabled )
				{
					value =
						'<a href="" onclick="showData(' +
						attributeIndex(attributes[i].dataNode) + ',' + i +
						',false);return false;" title="Show data">' +
						value + '</a>';
				}
				else if ( attributes[i].dataAll != undefined && dataEnabled )
				{
					value =
						'<a href="" onclick="showData(' +
						attributeIndex(attributes[i].dataAll) + ',' + i +
						',true);return false;" title="Show data">' +
						value + '</a>';
				}
				
				table +=
					'<tr><td><strong>' + attributes[i].displayName + ':</strong></td><td>' +
					value + '</td></tr>';
			}
		}
	}
	
	table += '</table>';
	detailsInfo.innerHTML = table;
	
	detailsExpand.disabled = !focusNode.hasChildren() || focusNode == selectedNode;
}

function setSelectedNode(newNode)
{
	if ( selectedNode && selectedNode.hasParent(newNode) )
	{
		zoomOut = true;
	}
	else
	{
		zoomOut = false;
	}
	
	selectedNodeLast = selectedNode;
	selectedNode = newNode;
	
	//if ( focusNode != selectedNode )
	{
		setFocus(selectedNode);
	}
}

function waitForData(dataWindow, target, title, time, postUrl, postVar)
{
	if ( nodeData.length == target )
	{
		if ( postUrl != undefined )
		{
			for ( var i = 0; i < nodeData.length; i++ )
			{
				nodeData[i] = nodeData[i].replace(/\n/g, ',');
			}
			
			var postString = nodeData.join('');
			postString = postString.slice(0, -1);
			
			dataWindow.document.body.removeChild(dataWindow.document.getElementById('loading'));
			document.body.removeChild(document.getElementById('data'));
			
			post(postUrl, postVar, postString, dataWindow);
		}
		else
		{
			//dataWindow.document.body.removeChild(dataWindow.document.getElementById('loading'));
			//document.body.removeChild(document.getElementById('data'));
			
			dataWindow.document.open();
			dataWindow.document.write('<pre>' + nodeData.join('') + '</pre>');
			dataWindow.document.close();
		}
		
		dataWindow.document.title = title; // replace after document.write()
	}
	else
	{
		var date = new Date();
		
		if ( date.getTime() - time > 10000 )
		{
			dataWindow.document.body.removeChild(dataWindow.document.getElementById('loading'));
			document.body.removeChild(document.getElementById('data'));
			dataWindow.document.body.innerHTML =
				'Timed out loading supplemental files for:<br/>' + document.location;
		}
		else
		{
			setTimeout(function() {waitForData(dataWindow, target, title, time, postUrl, postVar);}, 100);
		}
	}
}

function data(newData)
{
	nodeData.push(newData);
}

function enableData()
{
	dataEnabled = true;
}

function showData(indexData, indexAttribute, summary)
{
	var dataWindow = window.open('', '_blank');
	var title = 'Krona - ' + attributes[indexAttribute].displayName + ' - ' + focusNode.name;
	dataWindow.document.title = title;
	
	nodeData = new Array();
	
	if ( dataWindow && dataWindow.document && dataWindow.document.body != null )
	{
		//var loadImage = document.createElement('img');
		//loadImage.src = "file://localhost/Users/ondovb/Krona/KronaTools/img/loading.gif";
		//loadImage.id = "loading";
		//loadImage.alt = "Loading...";
		//dataWindow.document.body.appendChild(loadImage);
		dataWindow.document.body.innerHTML =
			'<img id="loading" src="' + loadingImage + '" alt="Loading..."></img>';
	}
	
	var scripts = document.createElement('div');
	scripts.id = 'data';
	document.body.appendChild(scripts);
	
	var files = focusNode.getData(indexData, summary);
	
	var date = new Date();
	var time = date.getTime();
	
	for ( var i = 0; i < files.length; i++ )
	{
		var script = document.createElement('script');
		script.src = files[i] + '?' + time;
		scripts.appendChild(script);
	}
	
	waitForData(dataWindow, files.length, title, time, attributes[indexAttribute].postUrl, attributes[indexAttribute].postVar);
	
	return false;
}

function showList(indexList, indexAttribute, summary)
{
	var list = focusNode.getList(indexList, summary);
	
	if ( attributes[indexAttribute].postUrl != undefined )
	{
		post(attributes[indexAttribute].postUrl, attributes[indexAttribute].postVar, list.join(','));
	}
	else
	{
		var dataWindow = window.open('', '_blank');
		
		if ( true || navigator.appName == 'Microsoft Internet Explorer' ) // :(
		{
			dataWindow.document.open();
			dataWindow.document.write('<pre>' + list.join('\n') + '</pre>');
			dataWindow.document.close();
		}
		else
		{
			var pre = document.createElement('pre');
			dataWindow.document.body.appendChild(pre);
			pre.innerHTML = list;
		}
		
		dataWindow.document.title = 'Krona - ' + attributes[indexAttribute].displayName + ' - ' + focusNode.name;
	}
}

function snapshot()
{
	svg = svgHeader();
	
	resetKeyOffset();
	
	snapshotMode = true;
	
	selectedNode.draw(false, true);
	selectedNode.draw(true, true);
	
	if ( focusNode != 0 && focusNode != selectedNode )
	{
		context.globalAlpha = 1;
		focusNode.drawHighlight(true);
	}
	
	if ( hueDisplayName && useHue() )
	{
		drawLegendSVG();
	}
	
	snapshotMode = false;
	
	svg += svgFooter();
	var dataUri = 'data:image/svg+xml,' + encodeURIComponent(svg)
	var string = '<html><body><iframe src="' + dataUri + '" frameborder="0" style="position:absolute; border:0; top:0px; left:0px; bottom:0px; right:0px; width:100%; height:100%;" allowfullscreen></iframe><a style="position:absolute" href="' + dataUri + '" download="snapshot.svg">Download Snapshot</a></html></body>';
    var win = window.open();
    win.document.write(string)
}

function save()
{
	alert(document.body.innerHTML);
}

function spacer()
{
	if ( snapshotMode )
	{
		return '&#160;&#160;&#160;';
	}
	else
	{
		return '   ';
	}
}

function suppressEvent(e)
{
	e.cancelBubble = true;
	if (e.stopPropagation) e.stopPropagation();
}

function svgFooter()
{
	return '</svg>';
}

function svgHeader()
{
	var patternWidth = fontSize * .6;//radius / 50;
	
	return '\
<?xml version="1.0" standalone="no"?>\
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" \
	"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">\
<svg width="' + imageWidth + '" height="' + imageHeight + '" version="1.1"\
	xmlns="http://www.w3.org/2000/svg">\
<title>Krona (snapshot) - ' +
(datasets > 1 ? datasetNames[currentDataset] + ' - ' : '') + selectedNode.name +
'</title>\
<defs>\
	<style type="text/css">\
	text {font-size: ' + fontSize + 'px; font-family: ' + fontFamily + '; dominant-baseline:central}\
	path {stroke-width:' + thinLineWidth * fontSize / 12 + ';}\
	path.wedge {stroke:none}\
	path.line {fill:none;stroke:black;}\
	line {stroke:black;stroke-width:' + thinLineWidth * fontSize / 12 + ';}\
	line.tick {stroke-width:' + thinLineWidth * fontSize / 6 + ';}\
	line.pattern {stroke-width:' + thinLineWidth * fontSize / 18 + ';}\
	circle {fill:none;stroke:black;stroke-width:' + thinLineWidth * fontSize / 12 + ';}\
	rect {stroke:black;stroke-width:' + thinLineWidth * fontSize / 12 + ';}\
	.highlight {stroke:black;stroke-width:'+ highlightLineWidth * fontSize / 12 + ';}\
	.searchHighlight {fill:rgb(255, 255, 100);stroke:none;}\
	</style>\
<pattern id="hiddenPattern" patternUnits="userSpaceOnUse" \
x="0" y="0" width="' + patternWidth + '" height="' + patternWidth + '">\
<line class="pattern" x1="0" y1="0" x2="' + patternWidth / 2 + '" y2="' + patternWidth / 2 + '"/>\
<line class="pattern" x1="' + patternWidth / 2 + '" y1="' + patternWidth +
'" x2="' + patternWidth + '" y2="' + patternWidth / 2 + '"/>\
</pattern>\
</defs>\
';
}

function svgText(text, x, y, anchor, bold, color)
{
	if ( typeof(anchor) == 'undefined' )
	{
		anchor = 'start';
	}
	
	if ( color == undefined )
	{
		color = 'black';
	}
	
	return '<text x="' + x + '" y="' + y +
		'" style="font-color:' + color + ';font-weight:' + (bold ? 'bold' : 'normal') +
		'" text-anchor="' + anchor + '">' + text + '</text>';
}

function toggleKeys()
{
	if ( showKeys )
	{
		keyControl.value = '…';
		showKeys = false;
	}
	else
	{
		keyControl.value = 'x';
		showKeys = true;
	}
	
	updateKeyControl();
	
	if ( progress == 1 )
	{
		draw();
	}
}

function update()
{
	if ( ! head )
	{
		return;
	}
	
	if ( mouseDown && focusNode != selectedNode )
	{
		var date = new Date();
		
		if ( date.getTime() - mouseDownTime > quickLookHoldLength )
		{
			if ( focusNode.hasChildren() )
			{
				expand(focusNode);
				quickLook = true;
			}
		}
	}
	
	if ( updateViewNeeded )
	{
		resize();
		mouseX = -1;
		mouseY = -1;
		
		collapse = collapseCheckBox.checked;
		showMagnitude = showMagnitudeCheckBox.checked;
		compress = true;//compressCheckBox.checked;
		shorten = true;//shortenCheckBox.checked;
		
		checkSelectedCollapse();
		updateMaxAbsoluteDepth();
		
		if ( focusNode.getCollapse() || focusNode.depth > maxAbsoluteDepth )
		{
			setFocus(selectedNode);
		}
		else
		{
			setFocus(focusNode);
		}
		
		updateView();
		
		updateViewNeeded = false;
	}
	
	var date = new Date();
	progress = (date.getTime() - tweenStartTime) / tweenLength;
//	progress += .01;
	
	if ( progress >= 1 )
	{
		progress = 1;
	}
	
	if ( progress != progressLast )
	{
		tweenFactor =// progress;
			(1 / (1 + Math.exp(-tweenCurvature * (progress - .5))) - .5) /
			(tweenMax - .5) / 2 + .5;
		
		if ( progress == 1 )
		{
			snapshotButton.disabled = false;
			zoomOut = false;
			
			//updateKeyControl();
			
			if ( ! quickLook )
			{
				//checkHighlight();
			}
			
			
			if ( fpsDisplay )
			{
				fpsDisplay.innerHTML = 'fps: ' + Math.round(tweenFrames * 1000 / tweenLength);
			}
		}
		
		draw();
	}
	
	progressLast = progress;
}

function updateDatasetButtons()
{
	if ( datasets == 1 )
	{
		return;
	}
	
	var node = selectedNode ? selectedNode : head;
	
	datasetButtonLast.disabled =
		node.attributes[magnitudeIndex][lastDataset] == 0;
	
	datasetButtonPrev.disabled = true;
	datasetButtonNext.disabled = true;
	
	for ( var i = 0; i < datasets; i++ )
	{
		var disable = node.attributes[magnitudeIndex][i] == 0;
		
		datasetDropDown.options[i].disabled = disable;
		
		if ( ! disable )
		{
			if ( i != currentDataset )
			{
				datasetButtonPrev.disabled = false;
				datasetButtonNext.disabled = false;
			}
		}
	}
}

function updateDatasetWidths()
{
	if ( datasets > 1 )
	{
		for ( var i = 0; i < datasets; i++ )
		{
			context.font = fontBold;
			var dim = context.measureText(datasetNames[i]);
			datasetWidths[i] = dim.width;
		}
	}
}

function updateKeyControl()
{
	if ( keys == 0 )//|| progress != 1 )
	{
		keyControl.style.visibility = 'hidden';
	}
	else
	{
		keyControl.style.visibility = 'visible';
		keyControl.style.right = margin + 'px';
		
		if ( showKeys )
		{
			keyControl.style.top =
				imageHeight -
				(
					keys * (keySize + keyBuffer) -
					keyBuffer +
					margin +
					keyControl.clientHeight * 1.5
				) + 'px';
		}
		else
		{
			keyControl.style.top =
				(imageHeight - margin - keyControl.clientHeight) + 'px';
		}
	}
}

function updateView()
{
	if ( selectedNode.depth > maxAbsoluteDepth - 1 )
	{
		maxAbsoluteDepth = selectedNode.depth + 1;
	}
	
	highlightedNode = selectedNode;
	
	angleFactor = 2 * Math.PI / (selectedNode.magnitude);
	
	maxPossibleDepth = Math.floor(gRadius / (fontSize * minRingWidthFactor));
	
	if ( maxPossibleDepth < 4 )
	{
		maxPossibleDepth = 4;
	}
	
	var minRadiusInner = fontSize * 8 / gRadius;
	var minRadiusFirst = fontSize * 6 / gRadius;
	var minRadiusOuter = fontSize * 5 / gRadius;
	
	if ( .25 < minRadiusInner )
	{
		minRadiusInner = .25;
	}
	
	if ( .15 < minRadiusFirst )
	{
		minRadiusFirst = .15;
	}
	
	if ( .15 < minRadiusOuter )
	{
		minRadiusOuter = .15;
	}
	
	// visibility of nodes depends on the depth they are displayed at,
	// so we need to set the max depth assuming they can all be displayed
	// and iterate it down based on the deepest child node we can display
	//
	var maxDepth;
	var newMaxDepth = selectedNode.getMaxDepth() - selectedNode.getDepth() + 1;
	//
	do
	{
		maxDepth = newMaxDepth;
		
		if ( ! compress && maxDepth > maxPossibleDepth )
		{
			maxDepth = maxPossibleDepth;
		}
		
		if ( compress )
		{
			compressedRadii = new Array(maxDepth);
			
			compressedRadii[0] = minRadiusInner;
			
			var offset = 0;
			
			while
			(
				lerp
				(
					Math.atan(offset + 2),
					Math.atan(offset + 1),
					Math.atan(maxDepth + offset - 1),
					minRadiusInner,
					1 - minRadiusOuter
				) - minRadiusInner > minRadiusFirst &&
				offset < 10
			)
			{
				offset++;
			}
			
			offset--;
			
			for ( var i = 1; i < maxDepth; i++ )
			{
				compressedRadii[i] = lerp
				(
					Math.atan(i + offset),
					Math.atan(offset),
					Math.atan(maxDepth + offset - 1),
					minRadiusInner,
					1 - minRadiusOuter
				)
			}
		}
		else
		{
			nodeRadius = 1 / maxDepth;
		}
		
		newMaxDepth = selectedNode.maxVisibleDepth(maxDepth);
		
		if ( compress )
		{
			if ( newMaxDepth <= maxPossibleDepth )
			{
//				compress
			}
		}
		else
		{
			if ( newMaxDepth > maxPossibleDepth )
			{
				newMaxDepth = maxPossibleDepth;
			}
		}
	}
	while ( newMaxDepth < maxDepth );
	
	maxDisplayDepth = maxDepth;
	
	lightnessFactor = (lightnessMax - lightnessBase) / (maxDepth > 8 ? 8 : maxDepth);
	keys = 0;
	
	nLabelOffsets = new Array(maxDisplayDepth - 1);
	labelOffsets = new Array(maxDisplayDepth - 1);
	labelLastNodes = new Array(maxDisplayDepth - 1);
	labelFirstNodes = new Array(maxDisplayDepth - 1);
	
	for ( var i = 0; i < maxDisplayDepth - 1; i++ )
	{
		if ( compress )
		{
			if ( i == maxDisplayDepth - 1 )
			{
				nLabelOffsets[i] = 0;
			}
			else
			{
				var width =
					(compressedRadii[i + 1] - compressedRadii[i]) *
					gRadius;
				
				nLabelOffsets[i] = Math.floor(width / fontSize / 1.2);
				
				if ( nLabelOffsets[i] > 2 )
				{
					nLabelOffsets[i] = min
					(
						Math.floor(width / fontSize / 1.75),
						5
					);
				}
			}
		}
		else
		{
			nLabelOffsets[i] = Math.max
			(
				Math.floor(Math.sqrt((nodeRadius * gRadius / fontSize)) * 1.5),
				3
			);
		}
		
		labelOffsets[i] = Math.floor((nLabelOffsets[i] - 1) / 2);
		labelLastNodes[i] = new Array(nLabelOffsets[i] + 1);
		labelFirstNodes[i] = new Array(nLabelOffsets[i] + 1);
		
		for ( var j = 0; j <= nLabelOffsets[i]; j++ )
		{
			// these arrays will allow nodes with neighboring labels to link to
			// each other to determine max label length
			
			labelLastNodes[i][j] = 0;
			labelFirstNodes[i][j] = 0;
		}
	}
	
	fontSizeText.innerHTML = fontSize;
	fontNormal = fontSize + 'px ' + fontFamily;
	context.font = fontNormal;
	fontBold = 'bold ' + fontSize + 'px ' + fontFamily;
	tickLength = fontSize * .7;
	
	head.setTargets(0);
	
	keySize = ((imageHeight - margin * 3) * 1 / 2) / keys * 3 / 4;
	
	if ( keySize > fontSize * maxKeySizeFactor )
	{
		keySize = fontSize * maxKeySizeFactor;
	}
	
	keyBuffer = keySize / 3;
	
	fontSizeLast = fontSize;
	
	if ( datasetChanged )
	{
		datasetChanged = false;
	}
	else
	{
		datasetAlpha.start = 0;
	}
	
	var date = new Date();
	tweenStartTime = date.getTime();
	progress = 0;
	tweenFrames = 0;
	
	updateKeyControl();
	updateDatasetWidths();
	
	document.title = 'Krona - ' + selectedNode.name;
	updateNavigationButtons();
	snapshotButton.disabled = true;
	
	maxAbsoluteDepthText.innerHTML = maxAbsoluteDepth - 1;
	
	maxAbsoluteDepthButtonDecrease.disabled = (maxAbsoluteDepth == 2);
	maxAbsoluteDepthButtonIncrease.disabled = (maxAbsoluteDepth == head.maxDepth);
	
	if ( collapse != collapseLast && search.value != '' )
	{
		onSearchChange();
		collapseLast = collapse;
	}
}

function updateMaxAbsoluteDepth()
{
	while ( maxAbsoluteDepth > 1 && selectedNode.depth > maxAbsoluteDepth - 1 )
	{
		selectedNode = selectedNode.getParent();
	}
}

function updateNavigationButtons()
{
	backButton.disabled = (nodeHistoryPosition == 0);
//	upButton.disabled = (selectedNode.getParent() == 0);
	forwardButton.disabled = (nodeHistoryPosition == nodeHistory.length);
}

function useHue()
{
	return useHueCheckBox && useHueCheckBox.checked;
}

function showMagnitudes()
{
	return showMagnitudesCheckBox && showMagnitudesCheckBox.checked;
}
/*
function zoomOut()
{
	return (
		selectedNodeLast != 0 &&
		selectedNodeLast.getDepth() < selectedNode.getDepth());
}
*/
  </script>
 </head>
 <body>
  <img id="hiddenImage" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAICAYAAADED76LAAAAAXNSR0IArs4c6QAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAALEwAACxMBAJqcGAAAAAd0SU1FB9oLCBQhNQwWVnsAAAAidEVYdENvbW1lbnQAQ3JlYXRlZCB3aXRoIEdJTVAgb24gYSBNYWOHqHdDAAABE0lEQVQYGQEIAff+AwAAABkAAAAAAAAA+gAAAAAAAAAAAAAAAAAAAAAAAAAMAwAAAAAAAAANAAAAAAAAAPoAAAAAAAAADAAAAAYAAAD0AwAAAPoAAAAAAAAAAAAAAPoAAAAMAAAADQAAAPoAAAD6AAAAAAAAAAAAAAAAAAAAAAwAAAAZAAAADAAAAAAAAAAAAAAAAAAAAAAAAAAADAAAABkAAAAMAAAAAAAAAAAAAAAAAAAAAAAAAAAMAAAAGQAAAAwAAAAAAAAADAAAAAwAAAAABAAAAAAAAAAAAAAA8wAAAPQAAAAAAAAAAAAAAA0AAAAAAAAAAAwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAwAAAAZRssKC5OpXwYAAAAASUVORK5CYII=" style="display:none" alt="Hidden Image"/>
  <img id="loadingImage" src="data:image/gif;base64,R0lGODlhEAAQAPIAAP///wAAAMLCwkJCQgAAAGJiYoKCgpKSkiH/C05FVFNDQVBFMi4wAwEAAAAh/hpDcmVhdGVkIHdpdGggYWpheGxvYWQuaW5mbwAh+QQJCgAAACwAAAAAEAAQAAADMwi63P4wyklrE2MIOggZnAdOmGYJRbExwroUmcG2LmDEwnHQLVsYOd2mBzkYDAdKa+dIAAAh+QQJCgAAACwAAAAAEAAQAAADNAi63P5OjCEgG4QMu7DmikRxQlFUYDEZIGBMRVsaqHwctXXf7WEYB4Ag1xjihkMZsiUkKhIAIfkECQoAAAAsAAAAABAAEAAAAzYIujIjK8pByJDMlFYvBoVjHA70GU7xSUJhmKtwHPAKzLO9HMaoKwJZ7Rf8AYPDDzKpZBqfvwQAIfkECQoAAAAsAAAAABAAEAAAAzMIumIlK8oyhpHsnFZfhYumCYUhDAQxRIdhHBGqRoKw0R8DYlJd8z0fMDgsGo/IpHI5TAAAIfkECQoAAAAsAAAAABAAEAAAAzIIunInK0rnZBTwGPNMgQwmdsNgXGJUlIWEuR5oWUIpz8pAEAMe6TwfwyYsGo/IpFKSAAAh+QQJCgAAACwAAAAAEAAQAAADMwi6IMKQORfjdOe82p4wGccc4CEuQradylesojEMBgsUc2G7sDX3lQGBMLAJibufbSlKAAAh+QQJCgAAACwAAAAAEAAQAAADMgi63P7wCRHZnFVdmgHu2nFwlWCI3WGc3TSWhUFGxTAUkGCbtgENBMJAEJsxgMLWzpEAACH5BAkKAAAALAAAAAAQABAAAAMyCLrc/jDKSatlQtScKdceCAjDII7HcQ4EMTCpyrCuUBjCYRgHVtqlAiB1YhiCnlsRkAAAOwAAAAAAAAAAAA==" style="display:none" alt="Loading Indicator"/>
  <img id="logo" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAANgAAAA8CAYAAAAE9XR5AAAC0WlDQ1BJQ0MgUHJvZmlsZQAAOI2NlM9LFGEYx7+zjRgoQWBme4ihQ0ioTBZlROWuv9i0bVl/lBLE7Oy7u5Ozs9PM7JoiEV46ZtE9Kg8e+gM8eOiUl8LALALpblFEgpeS7Xlnxt0R7ccLM/N5nx/f53nf4X2BGlkxTT0kAXnDsZJ9Uen66JhU+xEhHEEdwqhTVNuMJBIDoMFjsWtsvofAvyute/v/OurStpoHhP1A6Eea2Sqw7xfZC1lqBBC5XsOEYzrE9zhbnv0x55TH8659KNlFvEh8QDUtHv+auEPNKWmgRiRuyQZiUgHO60XV7+cgPfXMGB6k73Hq6S6ze3wWZtJKdz9xG/HnNOvu4ZrE8xmtN0bcTM9axuod9lg4oTmxIY9DI4YeH/C5yUjFr/qaoulEk9v6dmmwZ9t+S7mcIA4TJ8cL/TymkXI7p3JD1zwW9KlcV9znd1Yxyeseo5g5U3f/F/UWeoVR6GDQYNDbgIQk+hBFK0xYKCBDHo0iNLIyN8YitjG+Z6SORIAl8q9TzrqbcxtFyuZZI4jGMdNSUZDkD/JXeVV+Ks/JX2bDxeaqZ8a6qanLD76TLq+8ret7/Z48fZXqRsirI0vWfGVNdqDTQHcZYzZcVeI12P34ZmCVLFCpFSlXadytVHJ9Nr0jgWp/2j2KXZpebKrWWhUXbqzUL03v2KvCrlWxyqp2zqtxwXwmHhVPijGxQzwHSbwkdooXxW6anRcHKhnDpKJhwlWyoVCWgUnymjv+mRcL76y5o6GPGczSVImf/4RVyGg6CxzRf7j/c/B7xaOxIvDCBg6frto2ku4dIjQuV23OFeDCN7oP3lZtzXQeDj0BFs6oRavkSwvCG4pmdxw+6SqYk5aWzTlSuyyflSJ0JTEpZqhtLZKi65LrsiWL2cwqsXQb7Mypdk+lnnal5lO5vEHnr/YRsPWwXP75rFzeek49rAEv9d/AvP1FSOihagAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAALEwAACxMBAJqcGAAAAAd0SU1FB+AEEhYRJKJxkPUAACAASURBVHgBAGaAmX8B/////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAvUj3EAAAIABJREFUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA////AAAAAAD+/v4AAAAAAP///wD///8AAAAAAP///wAAAAAAAQEBAAEBAQAAAAAAAQEBAAICAgAAAAAAAQEBAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP///wAAAAAA/v7+AP7+/gD9/f0A/v7+AP39/QD+/v4A/f39AP39/QD9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AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAQEAAwMDAAUFBQALCwsALy4vAFhbWwC47+4As+rqAAAAAAAAAAAAAAABAAEA/wAAAAAA////AP///wD//wAA/v//AP7//wAA//8AAAD/AAAAAAD/AAAAAAAAAAQCAgADAwEABQUDAAIDAgACAwEAAgEBAAEBAwADAQIAAgEAAAQCAwADAgIAFQwfAGQ5jAD77O4A8tLVAEE/PwAiIiIAEBAQAAwMDAAHBwcAAgICAAEBAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEBAQACAgIACAgIAA0NDQA/Pz8A+/v7AKqpqQDw/f0AVxUVAAIA/wAAAAAAAAAAAP//AAD///4AAAABAAIBAQD+//4A////AP///wAAAAAAAAAAAAEAAAABAQEAAwMCAAAAAAAA/wAAAgECAAIDAwAAAAAAAQIAAAECAwD/AgIAAgECAP0C/ADH3rAAAwECADMzMQAsLCwAExMTABEREQAKCgoABQUFAAMDAwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA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AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD///8A/f39APz8/AD9/f0A+fn5APr6+gD6+voA+fn5APr6+gD6+voA+fn5APj5+AD9/P0AAgICAAYGBgAHBwcABgYGAAYGBgAICAgABgYGAAcHBwAGBgYABQUFAAMDAwACAgIAAgICAAEBAQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB/////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP///wAAAAAA/v7+AP7+/gD8/PwA/v7+APz8/AD8/PwA/P38AP38/QD7+/sA/Pz8AAMDAwAFBQUAAgICAAUFBQAEBAQAAwMDAAQEBAADAwMAAgICAAEBAQACAgIAAQEBAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAf////8AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD///8A/v7+AAAAAAD///8A////AP///wD9/f0A/v7+AAAAAAAAAAAAAQEBAAEBAQADAwMAAQEBAAEBAQABAQEAAgICAAAAAAABAQEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACanuzMvN2MUAAAAAElFTkSuQmCC" style="display:none" alt="Logo of Krona"/>
  <noscript>Javascript must be enabled to view this page.</noscript>
  <div style="display:none">
  <krona collapse="true" key="true">
   <attributes magnitude="magnitude">
    <attribute display="Total">magnitude</attribute>
    <attribute display="Unassigned">magnitudeUnassigned</attribute>
   </attributes>
   <datasets>
    <dataset>SRR14092160.b.krona</dataset>
   </datasets>
<node name="all">
 <magnitude><val>21424286</val></magnitude>
 <node name="k__Bacteria">
  <magnitude><val>21410566</val></magnitude>
  <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
  <node name="p__Vulcanimicrobiota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>10</val></magnitude>
   <node name="c__Vulcanimicrobiia">
    <magnitude><val>10</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Vulcanimicrobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>10</val></magnitude>
     <node name="f__Vulcanimicrobiaceae">
      <magnitude><val>10</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Vulcanimicrobium">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Vulcanimicrobium_alpinus">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Thermotogota">
   <magnitude><val>726</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Thermotogae">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>726</val></magnitude>
    <node name="o__Kosmotogales">
     <magnitude><val>38</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Kosmotogaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>38</val></magnitude>
      <node name="g__Mesotoga">
       <magnitude><val>38</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mesotoga_prima">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Mesotoga_infera">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Petrotogales">
     <magnitude><val>230</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Petrotogaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>230</val></magnitude>
      <node name="g__Marinitoga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>89</val></magnitude>
       <node name="s__Marinitoga_sp._BP5-C20A">
        <magnitude><val>89</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanotoga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Oceanotoga_sp._DSM_15011">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Tepiditoga">
       <magnitude><val>40</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tepiditoga_spiralis">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Defluviitoga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>83</val></magnitude>
       <node name="s__Defluviitoga_tunisiensis">
        <magnitude><val>83</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Thermotogales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>458</val></magnitude>
     <node name="f__Fervidobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>387</val></magnitude>
      <node name="g__Fervidobacterium">
       <magnitude><val>365</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fervidobacterium_pennivorans">
        <magnitude><val>341</val></magnitude>
       </node>
       <node name="s__Fervidobacterium_nodosum">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Thermosipho">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>22</val></magnitude>
       <node name="s__Thermosipho_africanus">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermotogaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>71</val></magnitude>
      <node name="g__Pseudothermotoga">
       <magnitude><val>61</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudothermotoga_thermarum">
        <magnitude><val>61</val></magnitude>
       </node>
      </node>
      <node name="g__Thermotoga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Thermotoga_petrophila">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Chlorobiota">
   <magnitude><val>252</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Chlorobiia">
    <magnitude><val>252</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Chlorobiales">
     <magnitude><val>252</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Chlorobiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>252</val></magnitude>
      <node name="g__Chlorobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Chlorobium_phaeobacteroides">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Chlorobium_phaeovibrioides">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Chlorobium_limicola">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Chlorobaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>91</val></magnitude>
       <node name="s__Chlorobaculum_tepidum">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Chlorobaculum_parvum">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Chlorobaculum_limnaeum">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Pelodictyon">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>102</val></magnitude>
       <node name="s__Pelodictyon_phaeoclathratiforme">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Pelodictyon_luteolum">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Prosthecochloris">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Prosthecochloris_sp._CIB_2401">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Prosthecochloris_sp._GSB1">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Calditrichota">
   <magnitude><val>23</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Calditrichia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>23</val></magnitude>
    <node name="o__Calditrichales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>23</val></magnitude>
     <node name="f__Calditrichaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>23</val></magnitude>
      <node name="g__Caldithrix">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Caldithrix_abyssi">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Fibrobacterota">
   <magnitude><val>47</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Fibrobacteria">
    <magnitude><val>47</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Fibrobacterales">
     <magnitude><val>47</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Fibrobacteraceae">
      <magnitude><val>47</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Fibrobacter">
       <magnitude><val>47</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fibrobacter_succinogenes">
        <magnitude><val>47</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Bdellovibrionota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>271</val></magnitude>
   <node name="c__Bacteriovoracia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>168</val></magnitude>
    <node name="o__Bacteriovoracales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>168</val></magnitude>
     <node name="f__Halobacteriovoraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>133</val></magnitude>
      <node name="g__Halobacteriovorax">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>133</val></magnitude>
       <node name="s__Halobacteriovorax_marinus">
        <magnitude><val>133</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bacteriovoracaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>35</val></magnitude>
      <node name="g__Bacteriovorax">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>35</val></magnitude>
       <node name="s__Bacteriovorax_stolpii">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Oligoflexia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>17</val></magnitude>
    <node name="o__Silvanigrellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>17</val></magnitude>
     <node name="f__Silvanigrellaceae">
      <magnitude><val>17</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pigmentibacter">
       <magnitude><val>17</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pigmentibacter_sp._JX0631">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Bdellovibrionia">
    <magnitude><val>86</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Bdellovibrionales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>86</val></magnitude>
     <node name="f__Pseudobdellovibrionaceae">
      <magnitude><val>86</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pseudobdellovibrio">
       <magnitude><val>30</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudobdellovibrio_exovorus">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Bdellovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>56</val></magnitude>
       <node name="s__Bdellovibrio_reynosensis">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Bdellovibrio_bacteriovorus">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="c__Deltaproteobacteria">
   <magnitude><val>406</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="g__Dissulfurimicrobium">
    <magnitude><val>297</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="s__Dissulfurimicrobium_hydrothermale">
     <magnitude><val>297</val></magnitude>
    </node>
   </node>
   <node name="o__Bradymonadales">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>109</val></magnitude>
    <node name="f__Bradymonadaceae">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>109</val></magnitude>
     <node name="g__Persicimonas">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>14</val></magnitude>
      <node name="s__Persicimonas_caeni">
       <magnitude><val>14</val></magnitude>
      </node>
     </node>
     <node name="g__Bradymonas">
      <magnitude><val>95</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Bradymonas_sediminis">
       <magnitude><val>95</val></magnitude>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Ignavibacteriota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>39</val></magnitude>
   <node name="c__Ignavibacteria">
    <magnitude><val>39</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Ignavibacteriales">
     <magnitude><val>39</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Ignavibacteriaceae">
      <magnitude><val>39</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Ignavibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>39</val></magnitude>
       <node name="s__Ignavibacterium_album">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Atribacterota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>17</val></magnitude>
   <node name="c__Atribacteria">
    <magnitude><val>17</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Atribacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>17</val></magnitude>
     <node name="f__Atribacteraceae">
      <magnitude><val>17</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Atribacter">
       <magnitude><val>17</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Atribacter_laminatus">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Deinococcota">
   <magnitude><val>363</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Deinococci">
    <magnitude><val>363</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Trueperales">
     <magnitude><val>65</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Trueperaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>65</val></magnitude>
      <node name="g__Truepera">
       <magnitude><val>65</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Truepera_radiovictrix">
        <magnitude><val>65</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Thermales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>97</val></magnitude>
     <node name="f__Thermaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>97</val></magnitude>
      <node name="g__Meiothermus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Meiothermus_taiwanensis">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Thermus">
       <magnitude><val>81</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermus_sp._CCB_US3_UF1">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Thermus_aquaticus">
        <magnitude><val>60</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Deinococcales">
     <magnitude><val>201</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Deinococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>201</val></magnitude>
      <node name="g__Deinococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>201</val></magnitude>
       <node name="s__Deinococcus_sp._KNUC1210">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Deinococcus_wulumuqiensis">
        <magnitude><val>115</val></magnitude>
       </node>
       <node name="s__Deinococcus_radiodurans">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Deinococcus_irradiatisoli">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Deinococcus_ficus">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Planctomycetota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>781</val></magnitude>
   <node name="c__Planctomycetia">
    <magnitude><val>439</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Pirellulales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>130</val></magnitude>
     <node name="f__Lacipirellulaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>55</val></magnitude>
      <node name="g__Lacipirellula">
       <magnitude><val>40</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lacipirellula_parvula">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Aeoliella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Aeoliella_mucimassa">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Pirellulaceae">
      <magnitude><val>75</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Anatilimnocola">
       <magnitude><val>46</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anatilimnocola_aggregata">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Stieleria">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Stieleria_neptunia">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Planctomycetales">
     <magnitude><val>231</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Planctomycetaceae">
      <magnitude><val>231</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Crateriforma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Crateriforma_conspicua">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Rubinisphaera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>147</val></magnitude>
       <node name="s__Rubinisphaera_brasiliensis">
        <magnitude><val>147</val></magnitude>
       </node>
      </node>
      <node name="g__Gimesia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Gimesia_panareensis">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Planctopirus">
       <magnitude><val>52</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Planctopirus_ephydatiae">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Isosphaerales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>54</val></magnitude>
     <node name="f__Isosphaeraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>54</val></magnitude>
      <node name="g__Paludisphaera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Paludisphaera_borealis">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Isosphaera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Isosphaera_pallida">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Gemmatales">
     <magnitude><val>24</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Gemmataceae">
      <magnitude><val>24</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gemmata">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Gemmata_obscuriglobus">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Frigoriglobus">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Frigoriglobus_tundricola">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Phycisphaerae">
    <magnitude><val>219</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Tepidisphaerales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11</val></magnitude>
     <node name="f__Tepidisphaeraceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Humisphaera">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Humisphaera_borealis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Sedimentisphaerales">
     <magnitude><val>208</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Anaerohalosphaeraceae">
      <magnitude><val>103</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Anaerohalosphaera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>103</val></magnitude>
       <node name="s__Anaerohalosphaera_lusitana">
        <magnitude><val>103</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sedimentisphaeraceae">
      <magnitude><val>105</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Sedimentisphaera">
       <magnitude><val>76</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sedimentisphaera_salicampi">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Sedimentisphaera_cyanobacteriorum">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Limihaloglobus">
       <magnitude><val>29</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Limihaloglobus_sulfuriphilus">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Candidatus_Brocadiia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>123</val></magnitude>
    <node name="o__Candidatus_Brocadiales">
     <magnitude><val>123</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Candidatus_Brocadiaceae">
      <magnitude><val>123</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Kuenenia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>123</val></magnitude>
       <node name="s__Candidatus_Kuenenia_stuttgartiensis">
        <magnitude><val>123</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Cyanobacteriota">
   <magnitude><val>2218</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Cyanophyceae">
    <magnitude><val>2218</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Gloeobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>336</val></magnitude>
     <node name="f__Gloeobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>336</val></magnitude>
      <node name="g__Gloeobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>336</val></magnitude>
       <node name="s__Gloeobacter_violaceus">
        <magnitude><val>325</val></magnitude>
       </node>
       <node name="s__Gloeobacter_kilaueensis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Pseudanabaenales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>196</val></magnitude>
     <node name="f__Pseudanabaenaceae">
      <magnitude><val>196</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pseudanabaena">
       <magnitude><val>196</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudanabaena_mucicola">
        <magnitude><val>76</val></magnitude>
       </node>
       <node name="s__Pseudanabaena_galeata">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Pseudanabaena_sp._Chao_1811">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Pseudanabaena_sp._PCC_7367">
        <magnitude><val>58</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Coleofasciculales">
     <magnitude><val>10</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Coleofasciculaceae">
      <magnitude><val>10</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Allocoleopsis">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Allocoleopsis_franciscana">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Synechococcales">
     <magnitude><val>304</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Synechococcaceae">
      <magnitude><val>195</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Dactylococcopsis">
       <magnitude><val>25</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dactylococcopsis_salina">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Synechococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>170</val></magnitude>
       <node name="s__Synechococcus_sp._ROS8604">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Synechococcus_sp._BIOS-U3-1">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Synechococcus_sp._CBW1004">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Synechococcus_sp._MIT_S9220">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Synechococcus_sp._JA-3-3Ab">
        <magnitude><val>63</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Prochlorococcaceae">
      <magnitude><val>109</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Prochlorococcus">
       <magnitude><val>109</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Prochlorococcus_marinus">
        <magnitude><val>109</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Thermostichales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>20</val></magnitude>
     <node name="f__Thermostichaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>20</val></magnitude>
      <node name="g__Thermostichus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Thermostichus_lividus">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Chroococcales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>809</val></magnitude>
     <node name="f__Aphanothecaceae">
      <magnitude><val>705</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Atelocyanobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>539</val></magnitude>
       <node name="s__Candidatus_Atelocyanobacterium_thalassa">
        <magnitude><val>539</val></magnitude>
       </node>
      </node>
      <node name="g__Gloeothece">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gloeothece_verrucosa">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Crocosphaera">
       <magnitude><val>144</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Crocosphaera_subtropica">
        <magnitude><val>144</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Geminocystaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>104</val></magnitude>
      <node name="g__Picosynechococcus">
       <magnitude><val>44</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Picosynechococcus_sp._PCC_7003">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Picosynechococcus_sp._PCC_7002">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Geminocystis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>60</val></magnitude>
       <node name="s__Geminocystis_sp._NIES-3709">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Geminocystis_herdmanii">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Pleurocapsales">
     <magnitude><val>77</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hyellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>77</val></magnitude>
      <node name="g__Pleurocapsa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>77</val></magnitude>
       <node name="s__Pleurocapsa_sp._PCC_7327">
        <magnitude><val>77</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Leptolyngbyales">
     <magnitude><val>267</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Trichocoleusaceae">
      <magnitude><val>65</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Trichocoleus">
       <magnitude><val>65</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Trichocoleus_desertorum">
        <magnitude><val>65</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Leptolyngbyaceae">
      <magnitude><val>202</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Kovacikia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>45</val></magnitude>
       <node name="s__Kovacikia_minuta">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Leptothermofonsia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>122</val></magnitude>
       <node name="s__Leptothermofonsia_sichuanensis">
        <magnitude><val>122</val></magnitude>
       </node>
      </node>
      <node name="g__Leptolyngbya">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>35</val></magnitude>
       <node name="s__Leptolyngbya_sp._7M">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Leptolyngbya_sp._BL0902">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Geitlerinematales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11</val></magnitude>
     <node name="f__Geitlerinemataceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Geitlerinema">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Geitlerinema_sp._PCC_7407">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Nostocales">
     <magnitude><val>148</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Nostocaceae">
      <magnitude><val>132</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nostoc">
       <magnitude><val>132</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nostoc_sp._TCL26-01">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Nostoc_sp._CENA543">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Nostoc_sphaeroides">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Nostoc_sp._PCC_7120_=_FACHB-418">
        <magnitude><val>64</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Calotrichaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>16</val></magnitude>
      <node name="g__Calothrix">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Calothrix_sp._PCC_6303">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Oscillatoriales">
     <magnitude><val>40</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Oscillatoriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>17</val></magnitude>
      <node name="g__Moorena">
       <magnitude><val>17</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Moorena_producens">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Microcoleaceae">
      <magnitude><val>23</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Planktothrix">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Planktothrix_agardhii">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Aquificota">
   <magnitude><val>58</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Aquificae">
    <magnitude><val>58</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Aquificales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>58</val></magnitude>
     <node name="f__Aquificaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>24</val></magnitude>
      <node name="g__Aquifex">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>24</val></magnitude>
       <node name="s__Aquifex_aeolicus">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Thermosulfidibacter">
      <magnitude><val>15</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Thermosulfidibacter_takaii">
       <magnitude><val>15</val></magnitude>
      </node>
     </node>
     <node name="f__Hydrogenothermaceae">
      <magnitude><val>19</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Persephonella">
       <magnitude><val>19</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Persephonella_marina">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Verrucomicrobiota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>1542298</val></magnitude>
   <node name="g__Methylacidimicrobium">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>25</val></magnitude>
    <node name="s__Methylacidimicrobium_sp._B4">
     <magnitude><val>25</val></magnitude>
    </node>
   </node>
   <node name="c__Opitutae">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>17</val></magnitude>
    <node name="o__Opitutales">
     <magnitude><val>17</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Opitutaceae">
      <magnitude><val>17</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Opitutus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Opitutus_terrae">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Verrucomicrobiae">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>1542256</val></magnitude>
    <node name="o__Verrucomicrobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1542256</val></magnitude>
     <node name="f__Verrucomicrobiaceae">
      <magnitude><val>72</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Roseimicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Roseimicrobium_sp._ORNL1">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Luteolibacter">
       <magnitude><val>47</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Luteolibacter_sp._SL250">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Luteolibacter_luteus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Verrucomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Verrucomicrobium_spinosum">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Akkermansiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1542184</val></magnitude>
      <node name="g__Akkermansia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1542184</val></magnitude>
       <node name="s__Akkermansia_massiliensis">
        <magnitude><val>625793</val></magnitude>
       </node>
       <node name="s__Akkermansia_glycaniphila">
        <magnitude><val>103</val></magnitude>
       </node>
       <node name="s__Akkermansia_muciniphila">
        <magnitude><val>30789</val></magnitude>
       </node>
       <node name="s__Akkermansia_sp._EB-AMDK43">
        <magnitude><val>778757</val></magnitude>
       </node>
       <node name="s__Akkermansia_biwaensis">
        <magnitude><val>106742</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Elusimicrobiota">
   <magnitude><val>1006</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Elusimicrobia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>509</val></magnitude>
    <node name="o__Elusimicrobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>509</val></magnitude>
     <node name="f__Elusimicrobiaceae">
      <magnitude><val>509</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Elusimicrobium">
       <magnitude><val>509</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Elusimicrobium_minutum">
        <magnitude><val>509</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Endomicrobiia">
    <magnitude><val>497</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Endomicrobiales">
     <magnitude><val>497</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Endomicrobiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>497</val></magnitude>
      <node name="g__Endomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>497</val></magnitude>
       <node name="s__Endomicrobium_proavitum">
        <magnitude><val>497</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Mycoplasmatota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>1920</val></magnitude>
   <node name="o__Mycoplasmoidales">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>1011</val></magnitude>
    <node name="f__Metamycoplasmataceae">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>978</val></magnitude>
     <node name="g__Mesomycoplasma">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>253</val></magnitude>
      <node name="s__Mesomycoplasma_ovipneumoniae">
       <magnitude><val>195</val></magnitude>
      </node>
      <node name="s__Mesomycoplasma_dispar">
       <magnitude><val>58</val></magnitude>
      </node>
     </node>
     <node name="g__Metamycoplasma">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>88</val></magnitude>
      <node name="s__Metamycoplasma_hominis">
       <magnitude><val>25</val></magnitude>
      </node>
      <node name="s__Metamycoplasma_orale">
       <magnitude><val>63</val></magnitude>
      </node>
     </node>
     <node name="g__Mycoplasmopsis">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>637</val></magnitude>
      <node name="s__Mycoplasmopsis_felis">
       <magnitude><val>19</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_edwardii">
       <magnitude><val>86</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_bovis">
       <magnitude><val>47</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_columboralis">
       <magnitude><val>246</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_meleagridis">
       <magnitude><val>67</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_citelli">
       <magnitude><val>57</val></magnitude>
      </node>
      <node name="s__Mycoplasmopsis_canis">
       <magnitude><val>115</val></magnitude>
      </node>
     </node>
    </node>
    <node name="f__Mycoplasmoidaceae">
     <magnitude><val>33</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Ureaplasma">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>33</val></magnitude>
      <node name="s__Ureaplasma_parvum">
       <magnitude><val>33</val></magnitude>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Mollicutes">
    <magnitude><val>863</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Entomoplasmatales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>611</val></magnitude>
     <node name="f__Spiroplasmataceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>245</val></magnitude>
      <node name="g__Spiroplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>245</val></magnitude>
       <node name="s__Spiroplasma_turonicum">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Spiroplasma_culicicola">
        <magnitude><val>221</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Entomoplasmataceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>366</val></magnitude>
      <node name="g__Mesoplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>366</val></magnitude>
       <node name="s__Mesoplasma_florum">
        <magnitude><val>366</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Mycoplasmatales">
     <magnitude><val>157</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Mycoplasmataceae">
      <magnitude><val>157</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Hepatoplasma">
       <magnitude><val>29</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Hepatoplasma_crinochetorum">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
      <node name="g__Mycoplasma">
       <magnitude><val>128</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mycoplasma_iguanae">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Mycoplasma_sp._OR1901">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Mycoplasma_sp._2045">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Acholeplasmatales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>95</val></magnitude>
     <node name="f__Acholeplasmataceae">
      <magnitude><val>95</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Acholeplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Acholeplasma_hippikon">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Acholeplasma_laidlawii">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Paracholeplasma">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paracholeplasma_brassicae">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Haploplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>50</val></magnitude>
       <node name="s__Haploplasma_axanthum">
        <magnitude><val>50</val></magnitude>
       </node>
      </node>
      <node name="g__Mariniplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Mariniplasma_anaerobium">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Candidatus_Izimaplasma">
    <magnitude><val>46</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Candidatus_Izemoplasmatales">
     <magnitude><val>46</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hujiaoplasmataceae">
      <magnitude><val>18</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Hujiaoplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Hujiaoplasma_nucleasis">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Candidatus_Izemoplasmataceae">
      <magnitude><val>28</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Xianfuyuplasma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Xianfuyuplasma_coldseepsis">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Spirochaetota">
   <magnitude><val>11332</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Spirochaetia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>11332</val></magnitude>
    <node name="o__Brachyspirales">
     <magnitude><val>1044</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Brachyspiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1044</val></magnitude>
      <node name="g__Brachyspira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1044</val></magnitude>
       <node name="s__Brachyspira_murdochii">
        <magnitude><val>103</val></magnitude>
       </node>
       <node name="s__Brachyspira_hampsonii">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Brachyspira_pilosicoli">
        <magnitude><val>653</val></magnitude>
       </node>
       <node name="s__Brachyspira_hyodysenteriae">
        <magnitude><val>217</val></magnitude>
       </node>
       <node name="s__Brachyspira_intermedia">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Leptospirales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>113</val></magnitude>
     <node name="f__Leptospiraceae">
      <magnitude><val>113</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Leptospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>113</val></magnitude>
       <node name="s__Leptospira_santarosai">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Leptospira_mayottensis">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Leptospira_biflexa">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Leptospira_noguchii">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Brevinematales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>26</val></magnitude>
     <node name="f__Thermospiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>26</val></magnitude>
      <node name="g__Thermospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Thermospira_aquatica">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Spirochaetales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>10149</val></magnitude>
     <node name="f__Treponemataceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>8917</val></magnitude>
      <node name="g__Treponema">
       <magnitude><val>8853</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Treponema_succinifaciens">
        <magnitude><val>116</val></magnitude>
       </node>
       <node name="s__Treponema_pedis">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Treponema_sp._Marseille-Q4132">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Treponema_vincentii">
        <magnitude><val>1004</val></magnitude>
       </node>
       <node name="s__Treponema_ruminis">
        <magnitude><val>619</val></magnitude>
       </node>
       <node name="s__Treponema_sp._OMZ_788">
        <magnitude><val>261</val></magnitude>
       </node>
       <node name="s__Treponema_medium">
        <magnitude><val>767</val></magnitude>
       </node>
       <node name="s__Treponema_socranskii">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Treponema_primitia">
        <magnitude><val>118</val></magnitude>
       </node>
       <node name="s__Treponema_brennaborense">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Treponema_parvum">
        <magnitude><val>425</val></magnitude>
       </node>
       <node name="s__Treponema_phagedenis">
        <magnitude><val>141</val></magnitude>
       </node>
       <node name="s__Treponema_denticola">
        <magnitude><val>3442</val></magnitude>
       </node>
       <node name="s__Treponema_putidum">
        <magnitude><val>957</val></magnitude>
       </node>
       <node name="s__Treponema_peruense">
        <magnitude><val>837</val></magnitude>
       </node>
      </node>
      <node name="g__Brucepastera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>64</val></magnitude>
       <node name="s__Brucepastera_parasyntrophica">
        <magnitude><val>64</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Borreliaceae">
      <magnitude><val>163</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Borrelia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>82</val></magnitude>
       <node name="s__Borrelia_sp._A-FGy1">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Borrelia_sp._HM">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Borrelia_hermsii">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Borrelia_puertoricensis">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Borreliella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>81</val></magnitude>
       <node name="s__Borreliella_californiensis">
        <magnitude><val>81</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Breznakiellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>124</val></magnitude>
      <node name="g__Gracilinema">
       <magnitude><val>18</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gracilinema_caldarium">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Breznakiella">
       <magnitude><val>68</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Breznakiella_homolactica">
        <magnitude><val>68</val></magnitude>
       </node>
      </node>
      <node name="g__Leadbettera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>38</val></magnitude>
       <node name="s__Leadbettera_azotonutricia">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sphaerochaetaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>268</val></magnitude>
      <node name="g__Parasphaerochaeta">
       <magnitude><val>91</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parasphaerochaeta_coccoides">
        <magnitude><val>91</val></magnitude>
       </node>
      </node>
      <node name="g__Sphaerochaeta">
       <magnitude><val>177</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sphaerochaeta_globosa">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__uncultured_Sphaerochaeta_sp.">
        <magnitude><val>85</val></magnitude>
       </node>
       <node name="s__Sphaerochaeta_pleomorpha">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Spirochaetaceae">
      <magnitude><val>677</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Marispirochaeta">
       <magnitude><val>200</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marispirochaeta_aestuarii">
        <magnitude><val>62</val></magnitude>
       </node>
       <node name="s__Marispirochaeta_sp.">
        <magnitude><val>138</val></magnitude>
       </node>
      </node>
      <node name="g__Thiospirochaeta">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thiospirochaeta_perfilievii">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Sediminispirochaeta">
       <magnitude><val>338</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sediminispirochaeta_smaragdinae">
        <magnitude><val>338</val></magnitude>
       </node>
      </node>
      <node name="g__Salinispira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Salinispira_pacifica">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanispirochaeta">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>101</val></magnitude>
       <node name="s__Oceanispirochaeta_crateris">
        <magnitude><val>101</val></magnitude>
       </node>
      </node>
      <node name="g__Entomospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Entomospira_entomophilus">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Balneolota">
   <magnitude><val>32</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Balneolia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>32</val></magnitude>
    <node name="o__Balneolales">
     <magnitude><val>32</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Cyclonatronaceae">
      <magnitude><val>32</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cyclonatronum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>32</val></magnitude>
       <node name="s__Cyclonatronum_proteinivorum">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Synergistota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>432</val></magnitude>
   <node name="c__Synergistia">
    <magnitude><val>432</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Synergistales">
     <magnitude><val>432</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Synergistaceae">
      <magnitude><val>86</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aminomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Aminomonas_paucivorans">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Thermanaerovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Thermanaerovibrio_acidaminovorans">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Cloacibacillus">
       <magnitude><val>58</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cloacibacillus_porcorum">
        <magnitude><val>58</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aminithiophilaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>22</val></magnitude>
      <node name="g__Aminithiophilus">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aminithiophilus_ramosus">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Dethiosulfovibrionaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>123</val></magnitude>
      <node name="g__Pyramidobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>96</val></magnitude>
       <node name="s__Pyramidobacter_piscolens">
        <magnitude><val>73</val></magnitude>
       </node>
       <node name="s__Pyramidobacter_sp._YE332">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Jonquetella">
       <magnitude><val>27</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Jonquetella_anthropi">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermovirgaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>45</val></magnitude>
      <node name="g__Thermovirga">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermovirga_lienii">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aminobacteriaceae">
      <magnitude><val>156</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Fretibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>74</val></magnitude>
       <node name="s__Fretibacterium_fastidiosum">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
      <node name="g__Aminobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>82</val></magnitude>
       <node name="s__Aminobacterium_sp._MB27-C1">
        <magnitude><val>82</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Bacillota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>15097285</val></magnitude>
   <node name="s__endosymbiont_'TC1'_of_Trimyema_compressum">
    <magnitude><val>35</val></magnitude>
   </node>
   <node name="c__Erysipelotrichia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>856844</val></magnitude>
    <node name="o__Erysipelotrichales">
     <magnitude><val>856844</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Coprobacillaceae">
      <magnitude><val>371710</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thomasclavelia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>362879</val></magnitude>
       <node name="s__Thomasclavelia_spiroformis">
        <magnitude><val>1885</val></magnitude>
       </node>
       <node name="s__Thomasclavelia_ramosa">
        <magnitude><val>336694</val></magnitude>
       </node>
       <node name="s__[Clostridium]_innocuum">
        <magnitude><val>24300</val></magnitude>
       </node>
      </node>
      <node name="g__Tannockella">
       <magnitude><val>95</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tannockella_kyphosi">
        <magnitude><val>95</val></magnitude>
       </node>
      </node>
      <node name="g__Catenibacterium">
       <magnitude><val>7354</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Catenibacterium_mitsuokai">
        <magnitude><val>5416</val></magnitude>
       </node>
       <node name="s__Catenibacterium_sp._co_0103">
        <magnitude><val>1938</val></magnitude>
       </node>
      </node>
      <node name="g__Faecalibacillus">
       <magnitude><val>1382</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Faecalibacillus_intestinalis">
        <magnitude><val>1382</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Erysipelotrichaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>484144</val></magnitude>
      <node name="g__Intestinibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>443</val></magnitude>
       <node name="s__Intestinibaculum_porci">
        <magnitude><val>443</val></magnitude>
       </node>
      </node>
      <node name="g__Bulleidia">
       <magnitude><val>170</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Bulleidia_sp._zg-1006">
        <magnitude><val>170</val></magnitude>
       </node>
      </node>
      <node name="g__Allocoprobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1481</val></magnitude>
       <node name="s__Allocoprobacillus_halotolerans">
        <magnitude><val>1481</val></magnitude>
       </node>
      </node>
      <node name="g__Erysipelothrix">
       <magnitude><val>562</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Erysipelothrix_sp._HDW6A">
        <magnitude><val>260</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_piscisicarius">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_inopinata">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_larvae">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_rhusiopathiae">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_sp._HDW6C">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Erysipelothrix_sp._HDW6B">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Allobaculum">
       <magnitude><val>544</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Allobaculum_mucilyticum">
        <magnitude><val>90</val></magnitude>
       </node>
       <node name="s__Allobaculum_sp._Allo2">
        <magnitude><val>454</val></magnitude>
       </node>
      </node>
      <node name="g__Faecalibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>180</val></magnitude>
       <node name="s__Faecalibaculum_rodentium">
        <magnitude><val>180</val></magnitude>
       </node>
      </node>
      <node name="g__Longicatena">
       <magnitude><val>77009</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Longicatena_caecimuris">
        <magnitude><val>77009</val></magnitude>
       </node>
      </node>
      <node name="g__Amedibacterium">
       <magnitude><val>403755</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Amedibacterium_intestinale">
        <magnitude><val>403755</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Turicibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>990</val></magnitude>
      <node name="g__Turicibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>990</val></magnitude>
       <node name="s__Turicibacter_sanguinis">
        <magnitude><val>118</val></magnitude>
       </node>
       <node name="s__Turicibacter_bilis">
        <magnitude><val>423</val></magnitude>
       </node>
       <node name="s__Turicibacter_sp._TJ11">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Turicibacter_sp._H121">
        <magnitude><val>418</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Bacilli">
    <magnitude><val>176541</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Lactobacillales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>129612</val></magnitude>
     <node name="f__Carnobacteriaceae">
      <magnitude><val>2125</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Carnobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>719</val></magnitude>
       <node name="s__Carnobacterium_divergens">
        <magnitude><val>72</val></magnitude>
       </node>
       <node name="s__Carnobacterium_maltaromaticum">
        <magnitude><val>489</val></magnitude>
       </node>
       <node name="s__Carnobacterium_inhibens">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Carnobacterium_sp._17-4">
        <magnitude><val>114</val></magnitude>
       </node>
      </node>
      <node name="g__Desemzia">
       <magnitude><val>52</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desemzia_incerta">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
      <node name="g__Jeotgalibaca">
       <magnitude><val>214</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Jeotgalibaca_arthritidis">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Jeotgalibaca_porci">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Jeotgalibaca_sp._MA1X17-3">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Jeotgalibaca_dankookensis">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Jeotgalibaca_ciconiae">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
      <node name="g__Marinilactibacillus">
       <magnitude><val>85</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marinilactibacillus_sp._15R">
        <magnitude><val>85</val></magnitude>
       </node>
      </node>
      <node name="g__Trichococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>162</val></magnitude>
       <node name="s__uncultured_Trichococcus_sp.">
        <magnitude><val>162</val></magnitude>
       </node>
      </node>
      <node name="g__Dolosigranulum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>37</val></magnitude>
       <node name="s__Dolosigranulum_pigrum">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
      <node name="g__Granulicatella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>856</val></magnitude>
       <node name="s__Granulicatella_elegans">
        <magnitude><val>78</val></magnitude>
       </node>
       <node name="s__Granulicatella_adiacens">
        <magnitude><val>778</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aerococcaceae">
      <magnitude><val>337</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aerococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>201</val></magnitude>
       <node name="s__Aerococcus_urinaehominis">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Aerococcus_christensenii">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Aerococcus_urinaeequi">
        <magnitude><val>104</val></magnitude>
       </node>
       <node name="s__Aerococcus_sanguinicola">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Globicatella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Globicatella_sanguinis">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Fundicoccus">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fundicoccus_culcitae">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Ignavigranum">
       <magnitude><val>71</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Ignavigranum_ruoffiae">
        <magnitude><val>71</val></magnitude>
       </node>
      </node>
      <node name="g__Suicoccus">
       <magnitude><val>24</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Suicoccus_acidiformans">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Abiotrophia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Abiotrophia_defectiva">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Streptococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>81475</val></magnitude>
      <node name="g__Floricoccus">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Floricoccus_penangensis">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Lactococcus">
       <magnitude><val>1329</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lactococcus_garvieae">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Lactococcus_raffinolactis">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Lactococcus_lactis">
        <magnitude><val>1055</val></magnitude>
       </node>
       <node name="s__Lactococcus_cremoris">
        <magnitude><val>211</val></magnitude>
       </node>
      </node>
      <node name="g__Streptococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>80112</val></magnitude>
       <node name="s__Streptococcus_toyakuensis">
        <magnitude><val>472</val></magnitude>
       </node>
       <node name="s__Streptococcus_chenjunshii">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Streptococcus_thermophilus">
        <magnitude><val>11913</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._KS_6">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._D7B5">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Streptococcus_pseudoporcinus">
        <magnitude><val>84</val></magnitude>
       </node>
       <node name="s__Streptococcus_gallolyticus">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._A12">
        <magnitude><val>2282</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._zg-86">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Streptococcus_parasanguinis">
        <magnitude><val>10893</val></magnitude>
       </node>
       <node name="s__Streptococcus_lactarius">
        <magnitude><val>391</val></magnitude>
       </node>
       <node name="s__Streptococcus_halotolerans">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Streptococcus_ferus">
        <magnitude><val>112</val></magnitude>
       </node>
       <node name="s__Streptococcus_equinus">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._LPB0220">
        <magnitude><val>1061</val></magnitude>
       </node>
       <node name="s__Streptococcus_oralis">
        <magnitude><val>1061</val></magnitude>
       </node>
       <node name="s__Streptococcus_pseudopneumoniae">
        <magnitude><val>139</val></magnitude>
       </node>
       <node name="s__Streptococcus_alactolyticus">
        <magnitude><val>334</val></magnitude>
       </node>
       <node name="s__Streptococcus_didelphis">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Streptococcus_pneumoniae">
        <magnitude><val>577</val></magnitude>
       </node>
       <node name="s__Streptococcus_pasteurianus">
        <magnitude><val>2359</val></magnitude>
       </node>
       <node name="s__Streptococcus_constellatus">
        <magnitude><val>1338</val></magnitude>
       </node>
       <node name="s__Streptococcus_porcinus">
        <magnitude><val>126</val></magnitude>
       </node>
       <node name="s__Streptococcus_australis">
        <magnitude><val>1573</val></magnitude>
       </node>
       <node name="s__Streptococcus_sobrinus">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._NPS_308">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Streptococcus_equi">
        <magnitude><val>329</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._Marseille-Q6470">
        <magnitude><val>241</val></magnitude>
       </node>
       <node name="s__Streptococcus_mitis">
        <magnitude><val>977</val></magnitude>
       </node>
       <node name="s__Streptococcus_himalayensis">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._NSJ-72">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Streptococcus_parasuis">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._DTU_2020_1000888_1_SI_GRL_NUU_041A">
        <magnitude><val>101</val></magnitude>
       </node>
       <node name="s__Streptococcus_marmotae">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._1643">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Streptococcus_iniae">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._29887">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Streptococcus_respiraculi">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Streptococcus_parauberis">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Streptococcus_pantholopis">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Streptococcus_cristatus">
        <magnitude><val>223</val></magnitude>
       </node>
       <node name="s__Streptococcus_anginosus">
        <magnitude><val>4818</val></magnitude>
       </node>
       <node name="s__Streptococcus_vestibularis">
        <magnitude><val>203</val></magnitude>
       </node>
       <node name="s__Streptococcus_pluranimalium">
        <magnitude><val>53</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._116-D4">
        <magnitude><val>98</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._oral_taxon_431">
        <magnitude><val>143</val></magnitude>
       </node>
       <node name="s__Streptococcus_gordonii">
        <magnitude><val>369</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._FDAARGOS_192">
        <magnitude><val>780</val></magnitude>
       </node>
       <node name="s__Streptococcus_uberis">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Streptococcus_lutetiensis">
        <magnitude><val>222</val></magnitude>
       </node>
       <node name="s__Streptococcus_sanguinis">
        <magnitude><val>1094</val></magnitude>
       </node>
       <node name="s__Streptococcus_mutans">
        <magnitude><val>144</val></magnitude>
       </node>
       <node name="s__Streptococcus_agalactiae">
        <magnitude><val>777</val></magnitude>
       </node>
       <node name="s__Streptococcus_infantis">
        <magnitude><val>137</val></magnitude>
       </node>
       <node name="s__Streptococcus_infantarius">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._oral_taxon_061">
        <magnitude><val>303</val></magnitude>
       </node>
       <node name="s__Streptococcus_gwangjuense">
        <magnitude><val>110</val></magnitude>
       </node>
       <node name="s__Streptococcus_rubneri">
        <magnitude><val>505</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._Marseille-Q3533">
        <magnitude><val>178</val></magnitude>
       </node>
       <node name="s__Streptococcus_dysgalactiae">
        <magnitude><val>123</val></magnitude>
       </node>
       <node name="s__Streptococcus_acidominimus">
        <magnitude><val>1193</val></magnitude>
       </node>
       <node name="s__Streptococcus_periodonticum">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Streptococcus_koreensis">
        <magnitude><val>569</val></magnitude>
       </node>
       <node name="s__Streptococcus_ratti">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Streptococcus_pyogenes">
        <magnitude><val>5413</val></magnitude>
       </node>
       <node name="s__Streptococcus_salivarius">
        <magnitude><val>21618</val></magnitude>
       </node>
       <node name="s__Streptococcus_oriscaviae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Streptococcus_intermedius">
        <magnitude><val>124</val></magnitude>
       </node>
       <node name="s__Streptococcus_ilei">
        <magnitude><val>1312</val></magnitude>
       </node>
       <node name="s__Streptococcus_canis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Streptococcus_ruminicola">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Streptococcus_suis">
        <magnitude><val>1966</val></magnitude>
       </node>
       <node name="s__Streptococcus_sp._DTU_2020_1001019_1_SI_AUS_MUR_006">
        <magnitude><val>138</val></magnitude>
       </node>
       <node name="s__Streptococcus_merionis">
        <magnitude><val>203</val></magnitude>
       </node>
       <node name="s__Streptococcus_milleri">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Enterococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>32761</val></magnitude>
      <node name="g__Enterococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>31841</val></magnitude>
       <node name="s__Enterococcus_rotai">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Enterococcus_gallinarum">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Enterococcus_faecium">
        <magnitude><val>27589</val></magnitude>
       </node>
       <node name="s__Enterococcus_cecorum">
        <magnitude><val>2231</val></magnitude>
       </node>
       <node name="s__Enterococcus_thailandicus">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Enterococcus_faecalis">
        <magnitude><val>1540</val></magnitude>
       </node>
       <node name="s__Enterococcus_avium">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Enterococcus_mundtii">
        <magnitude><val>94</val></magnitude>
       </node>
       <node name="s__Enterococcus_raffinosus">
        <magnitude><val>81</val></magnitude>
       </node>
       <node name="s__Enterococcus_hirae">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Enterococcus_casseliflavus">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Enterococcus_saigonensis">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Enterococcus_wangshanyuanii">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Enterococcus_durans">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Enterococcus_saccharolyticus">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Tetragenococcus">
       <magnitude><val>577</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tetragenococcus_halophilus">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Tetragenococcus_koreensis">
        <magnitude><val>475</val></magnitude>
       </node>
      </node>
      <node name="g__Melissococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Melissococcus_plutonius">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Vagococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>330</val></magnitude>
       <node name="s__Vagococcus_intermedius">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Vagococcus_penaei">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Vagococcus_luciliae">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Vagococcus_fluvialis">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Vagococcus_zengguangii">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Vagococcus_xieshaowenii">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Vagococcus_lutrae">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Lactobacillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>12914</val></magnitude>
      <node name="g__Schleiferilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>40</val></magnitude>
       <node name="s__Schleiferilactobacillus_harbinensis">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Ligilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>5425</val></magnitude>
       <node name="s__Ligilactobacillus_salivarius">
        <magnitude><val>389</val></magnitude>
       </node>
       <node name="s__Ligilactobacillus_ruminis">
        <magnitude><val>4524</val></magnitude>
       </node>
       <node name="s__Ligilactobacillus_cholophilus">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Ligilactobacillus_murinus">
        <magnitude><val>424</val></magnitude>
       </node>
       <node name="s__Ligilactobacillus_saerimneri">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Ligilactobacillus_acidipiscis">
        <magnitude><val>59</val></magnitude>
       </node>
      </node>
      <node name="g__Lactobacillus">
       <magnitude><val>2386</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lactobacillus_helveticus">
        <magnitude><val>72</val></magnitude>
       </node>
       <node name="s__Lactobacillus_johnsonii">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Lactobacillus_sp._KimC2">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Lactobacillus_amylolyticus">
        <magnitude><val>126</val></magnitude>
       </node>
       <node name="s__Lactobacillus_amylovorus">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Lactobacillus_crispatus">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Lactobacillus_panisapium">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Lactobacillus_sp._Kim32-2">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Lactobacillus_kullabergensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Lactobacillus_isalae">
        <magnitude><val>644</val></magnitude>
       </node>
       <node name="s__Lactobacillus_sp._ESL0785">
        <magnitude><val>73</val></magnitude>
       </node>
       <node name="s__Lactobacillus_iners">
        <magnitude><val>368</val></magnitude>
       </node>
       <node name="s__Lactobacillus_sp._IBH004">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Lactobacillus_acidophilus">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Lactobacillus_delbrueckii">
        <magnitude><val>62</val></magnitude>
       </node>
       <node name="s__Lactobacillus_apis">
        <magnitude><val>636</val></magnitude>
       </node>
      </node>
      <node name="g__Apilactobacillus">
       <magnitude><val>202</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Apilactobacillus_apisilvae">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Apilactobacillus_apinorum">
        <magnitude><val>160</val></magnitude>
       </node>
       <node name="s__Apilactobacillus_bombintestini">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Weissella">
       <magnitude><val>1086</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Weissella_cibaria">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Weissella_diestrammenae">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Weissella_ceti">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__Weissella_confusa">
        <magnitude><val>899</val></magnitude>
       </node>
       <node name="s__Weissella_paramesenteroides">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Weissella_soli">
        <magnitude><val>89</val></magnitude>
       </node>
      </node>
      <node name="g__Paucilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27</val></magnitude>
       <node name="s__Paucilactobacillus_hokkaidonensis">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Nicoliella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Nicoliella_spurrieriana">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Liquorilactobacillus">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Liquorilactobacillus_mali">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Companilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>452</val></magnitude>
       <node name="s__Companilactobacillus_zhachilii">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Companilactobacillus_ginsenosidimutans">
        <magnitude><val>291</val></magnitude>
       </node>
       <node name="s__Companilactobacillus_farciminis">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Companilactobacillus_paralimentarius">
        <magnitude><val>106</val></magnitude>
       </node>
       <node name="s__Companilactobacillus_pabuli">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Companilactobacillus_heilongjiangensis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Lentilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>255</val></magnitude>
       <node name="s__Lentilactobacillus_hilgardii">
        <magnitude><val>112</val></magnitude>
       </node>
       <node name="s__Lentilactobacillus_curieae">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Lentilactobacillus_laojiaonis">
        <magnitude><val>133</val></magnitude>
       </node>
      </node>
      <node name="g__Levilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>182</val></magnitude>
       <node name="s__Levilactobacillus_brevis">
        <magnitude><val>182</val></magnitude>
       </node>
      </node>
      <node name="g__Fructilactobacillus">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fructilactobacillus_sanfranciscensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Fructilactobacillus_lindneri">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Leuconostoc">
       <magnitude><val>106</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leuconostoc_mesenteroides">
        <magnitude><val>106</val></magnitude>
       </node>
      </node>
      <node name="g__Limosilactobacillus">
       <magnitude><val>1042</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Limosilactobacillus_frumenti">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_fermentum">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_reuteri">
        <magnitude><val>327</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_gastricus">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_vaginalis">
        <magnitude><val>537</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_pontis">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Limosilactobacillus_mucosae">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Lacticaseibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>885</val></magnitude>
       <node name="s__Lacticaseibacillus_paracasei">
        <magnitude><val>455</val></magnitude>
       </node>
       <node name="s__Lacticaseibacillus_rhamnosus">
        <magnitude><val>163</val></magnitude>
       </node>
       <node name="s__Lacticaseibacillus_manihotivorans">
        <magnitude><val>135</val></magnitude>
       </node>
       <node name="s__Lacticaseibacillus_zeae">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Lacticaseibacillus_sp._KACC_23028">
        <magnitude><val>73</val></magnitude>
       </node>
      </node>
      <node name="g__Furfurilactobacillus">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Furfurilactobacillus_rossiae">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Lactiplantibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>229</val></magnitude>
       <node name="s__Lactiplantibacillus_plantarum">
        <magnitude><val>166</val></magnitude>
       </node>
       <node name="s__Lactiplantibacillus_pentosus">
        <magnitude><val>63</val></magnitude>
       </node>
      </node>
      <node name="g__Amylolactobacillus">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Amylolactobacillus_amylophilus">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Loigolactobacillus">
       <magnitude><val>43</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Loigolactobacillus_coryniformis">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Loigolactobacillus_backii">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Latilactobacillus">
       <magnitude><val>246</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Latilactobacillus_sakei">
        <magnitude><val>93</val></magnitude>
       </node>
       <node name="s__Latilactobacillus_curvatus">
        <magnitude><val>98</val></magnitude>
       </node>
       <node name="s__Latilactobacillus_fuchuensis">
        <magnitude><val>55</val></magnitude>
       </node>
      </node>
      <node name="g__Secundilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>30</val></magnitude>
       <node name="s__Secundilactobacillus_malefermentans">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Pediococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>190</val></magnitude>
       <node name="s__Pediococcus_acidilactici">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Pediococcus_damnosus">
        <magnitude><val>85</val></magnitude>
       </node>
       <node name="s__Pediococcus_inopinatus">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Pediococcus_claussenii">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Bombilactobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Bombilactobacillus_bombi">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Bacillales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>46929</val></magnitude>
     <node name="f__Gemellaceae">
      <magnitude><val>1810</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gemella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1810</val></magnitude>
       <node name="s__Gemella_sanguinis">
        <magnitude><val>1566</val></magnitude>
       </node>
       <node name="s__Gemella_haemolysans">
        <magnitude><val>151</val></magnitude>
       </node>
       <node name="s__Gemella_morbillorum">
        <magnitude><val>93</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bacillaceae">
      <magnitude><val>22591</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Domibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>94</val></magnitude>
       <node name="s__Domibacillus_sp._DTU_2020_1001157_1_SI_ALB_TIR_016">
        <magnitude><val>94</val></magnitude>
       </node>
      </node>
      <node name="g__Radiobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>412</val></magnitude>
       <node name="s__Radiobacillus_deserti">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Radiobacillus_kanasensis">
        <magnitude><val>389</val></magnitude>
       </node>
      </node>
      <node name="g__Salipaludibacillus">
       <magnitude><val>100</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Salipaludibacillus_sp._LMS25">
        <magnitude><val>100</val></magnitude>
       </node>
      </node>
      <node name="g__Rossellomorea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>609</val></magnitude>
       <node name="s__Rossellomorea_marisflavi">
        <magnitude><val>465</val></magnitude>
       </node>
       <node name="s__Rossellomorea_vietnamensis">
        <magnitude><val>144</val></magnitude>
       </node>
      </node>
      <node name="g__Halobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>818</val></magnitude>
       <node name="s__Halobacillus_naozhouensis">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Halobacillus_mangrovi">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Halobacillus_shinanisalinarum">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Halobacillus_litoralis">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Halobacillus_salinarum">
        <magnitude><val>514</val></magnitude>
       </node>
       <node name="s__Halobacillus_amylolyticus">
        <magnitude><val>94</val></magnitude>
       </node>
      </node>
      <node name="g__Paenalkalicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>24</val></magnitude>
       <node name="s__Paenalkalicoccus_suaedae">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Niallia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>853</val></magnitude>
       <node name="s__Niallia_sp._Man26">
        <magnitude><val>212</val></magnitude>
       </node>
       <node name="s__Niallia_circulans">
        <magnitude><val>180</val></magnitude>
       </node>
       <node name="s__Niallia_taxi">
        <magnitude><val>404</val></magnitude>
       </node>
       <node name="s__Niallia_sp._RD1">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Cytobacillus">
       <magnitude><val>514</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cytobacillus_kochii">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Cytobacillus_gottheilii">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Cytobacillus_firmus">
        <magnitude><val>123</val></magnitude>
       </node>
       <node name="s__Cytobacillus_pseudoceanisediminis">
        <magnitude><val>188</val></magnitude>
       </node>
       <node name="s__Cytobacillus_spongiae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Cytobacillus_solani">
        <magnitude><val>114</val></magnitude>
       </node>
      </node>
      <node name="g__Psychrobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>37</val></magnitude>
       <node name="s__Psychrobacillus_sp._INOP01">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
      <node name="g__Paraliobacillus">
       <magnitude><val>65</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paraliobacillus_zengyii">
        <magnitude><val>65</val></magnitude>
       </node>
      </node>
      <node name="g__Alkalihalobacillus">
       <magnitude><val>329</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Alkalihalobacillus_sp._LMS39">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Alkalihalobacillus_sp._AL-G">
        <magnitude><val>296</val></magnitude>
       </node>
      </node>
      <node name="g__Neobacillus">
       <magnitude><val>1420</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Neobacillus_sp._Marseille-Q6967">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._SuZ13">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._OS1-32">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Neobacillus_cucumis">
        <magnitude><val>219</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._YX16">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._PS2-9">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._PS3-12">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._OS1-2">
        <magnitude><val>109</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._OS1-33">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Neobacillus_mesonae">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._DY30">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._PS3-34">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._PS3-40">
        <magnitude><val>231</val></magnitude>
       </node>
       <node name="s__Neobacillus_drentensis">
        <magnitude><val>181</val></magnitude>
       </node>
       <node name="s__Neobacillus_sp._114">
        <magnitude><val>154</val></magnitude>
       </node>
       <node name="s__Neobacillus_novalis">
        <magnitude><val>82</val></magnitude>
       </node>
      </node>
      <node name="g__Lentibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>460</val></magnitude>
       <node name="s__Lentibacillus_amyloliquefaciens">
        <magnitude><val>409</val></magnitude>
       </node>
       <node name="s__Lentibacillus_daqui">
        <magnitude><val>51</val></magnitude>
       </node>
      </node>
      <node name="g__Fervidibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Fervidibacillus_halotolerans">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Ectobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>40</val></magnitude>
       <node name="s__Ectobacillus_sp._JY-23">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Halalkalibacterium_(ex_Joshi_et_al._2022)">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Halalkalibacterium_halodurans">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Lederbergia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Lederbergia_lenta">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
      <node name="g__Terribacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>115</val></magnitude>
       <node name="s__Terribacillus_sp._DMT04">
        <magnitude><val>115</val></magnitude>
       </node>
      </node>
      <node name="g__Metabacillus">
       <magnitude><val>468</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Metabacillus_endolithicus">
        <magnitude><val>91</val></magnitude>
       </node>
       <node name="s__Metabacillus_sediminilitoris">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Metabacillus_sp._cB07">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Metabacillus_sp._KUDC1714">
        <magnitude><val>261</val></magnitude>
       </node>
      </node>
      <node name="g__Salicibibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>96</val></magnitude>
       <node name="s__Salicibibacter_halophilus">
        <magnitude><val>96</val></magnitude>
       </node>
      </node>
      <node name="g__Salimicrobium">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Salimicrobium_jeotgali">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Priestia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>323</val></magnitude>
       <node name="s__Priestia_aryabhattai">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Priestia_flexa">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Priestia_megaterium">
        <magnitude><val>231</val></magnitude>
       </node>
       <node name="s__Priestia_koreensis">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Priestia_filamentosa">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Sutcliffiella">
       <magnitude><val>97</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sutcliffiella_horikoshii">
        <magnitude><val>97</val></magnitude>
       </node>
      </node>
      <node name="g__Pontibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>82</val></magnitude>
       <node name="s__Pontibacillus_sp._HMF3514">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Pontibacillus_chungwhensis">
        <magnitude><val>55</val></magnitude>
       </node>
      </node>
      <node name="g__Allobacillus">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Allobacillus_halotolerans">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Virgibacillus">
       <magnitude><val>681</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Virgibacillus_dokdonensis">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Virgibacillus_natechei">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Virgibacillus_sp._MSP4-1">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Virgibacillus_necropolis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Virgibacillus_sp._SK37">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Virgibacillus_sp._NKC19-16">
        <magnitude><val>392</val></magnitude>
       </node>
       <node name="s__Virgibacillus_sp._Bac330">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Virgibacillus_halodenitrificans">
        <magnitude><val>145</val></magnitude>
       </node>
      </node>
      <node name="g__Aeribacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>51</val></magnitude>
       <node name="s__Aeribacillus_pallidus">
        <magnitude><val>51</val></magnitude>
       </node>
      </node>
      <node name="g__Gracilibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>113</val></magnitude>
       <node name="s__Gracilibacillus_salinarum">
        <magnitude><val>65</val></magnitude>
       </node>
       <node name="s__Gracilibacillus_caseinilyticus">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Gracilibacillus_salitolerans">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Geobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>320</val></magnitude>
       <node name="s__Geobacillus_genomosp._3">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Geobacillus_subterraneus">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Geobacillus_stearothermophilus">
        <magnitude><val>224</val></magnitude>
       </node>
      </node>
      <node name="g__Evansella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>60</val></magnitude>
       <node name="s__Evansella_sp._LMS18">
        <magnitude><val>60</val></magnitude>
       </node>
      </node>
      <node name="g__Heyndrickxia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>579</val></magnitude>
       <node name="s__Heyndrickxia_coagulans">
        <magnitude><val>496</val></magnitude>
       </node>
       <node name="s__Heyndrickxia_oleronia">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Heyndrickxia_vini">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Caldibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>111</val></magnitude>
       <node name="s__Caldibacillus_thermoamylovorans">
        <magnitude><val>111</val></magnitude>
       </node>
      </node>
      <node name="g__Sediminibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>49</val></magnitude>
       <node name="s__Sediminibacillus_dalangtanensis">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
      <node name="g__Salisediminibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>253</val></magnitude>
       <node name="s__Salisediminibacterium_selenitireducens">
        <magnitude><val>235</val></magnitude>
       </node>
       <node name="s__Salisediminibacterium_beveridgei">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Peribacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1449</val></magnitude>
       <node name="s__Peribacillus_butanolivorans">
        <magnitude><val>379</val></magnitude>
       </node>
       <node name="s__Peribacillus_sp._R9-11">
        <magnitude><val>163</val></magnitude>
       </node>
       <node name="s__Peribacillus_psychrosaccharolyticus">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Peribacillus_frigoritolerans">
        <magnitude><val>111</val></magnitude>
       </node>
       <node name="s__Peribacillus_asahii">
        <magnitude><val>459</val></magnitude>
       </node>
       <node name="s__Peribacillus_simplex">
        <magnitude><val>154</val></magnitude>
       </node>
       <node name="s__Peribacillus_muralis">
        <magnitude><val>119</val></magnitude>
       </node>
      </node>
      <node name="g__Shouchella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>108</val></magnitude>
       <node name="s__Shouchella_lehensis">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Shouchella_clausii">
        <magnitude><val>70</val></magnitude>
       </node>
      </node>
      <node name="g__Caldalkalibacillus">
       <magnitude><val>92</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caldalkalibacillus_thermarum">
        <magnitude><val>92</val></magnitude>
       </node>
      </node>
      <node name="g__Mesobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>656</val></magnitude>
       <node name="s__Mesobacillus_foraminis">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Mesobacillus_subterraneus">
        <magnitude><val>133</val></magnitude>
       </node>
       <node name="s__Mesobacillus_sp._AQ2">
        <magnitude><val>116</val></magnitude>
       </node>
       <node name="s__Mesobacillus_sp._S13">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Mesobacillus_jeotgali">
        <magnitude><val>362</val></magnitude>
       </node>
      </node>
      <node name="g__Pradoshia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>59</val></magnitude>
       <node name="s__Pradoshia_sp._D12">
        <magnitude><val>59</val></magnitude>
       </node>
      </node>
      <node name="g__Parageobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2364</val></magnitude>
       <node name="s__Parageobacillus_sp._KH3-4">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Parageobacillus_thermoglucosidasius">
        <magnitude><val>535</val></magnitude>
       </node>
       <node name="s__Parageobacillus_toebii">
        <magnitude><val>1796</val></magnitude>
       </node>
      </node>
      <node name="g__Amphibacillus">
       <magnitude><val>57</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Amphibacillus_xylanus">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Lysinibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>555</val></magnitude>
       <node name="s__Lysinibacillus_sp._2017">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_sp._Ag94">
        <magnitude><val>117</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_fusiformis">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_sp._CD3-6">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_pakistanensis">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_agricola">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_sp._SGAir0095">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_irui">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_sp._PLM2">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_sp._OF-1">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Lysinibacillus_timonensis">
        <magnitude><val>59</val></magnitude>
       </node>
      </node>
      <node name="g__Bacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>6233</val></magnitude>
       <node name="s__Bacillus_gobiensis">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Bacillus_altitudinis">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._S3">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Bacillus_smithii">
        <magnitude><val>186</val></magnitude>
       </node>
       <node name="s__Bacillus_tequilensis">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._FJAT-42376">
        <magnitude><val>264</val></magnitude>
       </node>
       <node name="s__Bacillus_badius">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._HSf4">
        <magnitude><val>82</val></magnitude>
       </node>
       <node name="s__Bacillus_velezensis">
        <magnitude><val>1336</val></magnitude>
       </node>
       <node name="s__Bacillus_safensis">
        <magnitude><val>65</val></magnitude>
       </node>
       <node name="s__Bacillus_cereus">
        <magnitude><val>1322</val></magnitude>
       </node>
       <node name="s__Bacillus_pseudomycoides">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Bacillus_aquiflavi">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Bacillus_mojavensis">
        <magnitude><val>80</val></magnitude>
       </node>
       <node name="s__Bacillus_cytotoxicus">
        <magnitude><val>105</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._DX3.1">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Bacillus_carboniphilus">
        <magnitude><val>70</val></magnitude>
       </node>
       <node name="s__Bacillus_atrophaeus">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Bacillus_spizizenii">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Bacillus_thuringiensis">
        <magnitude><val>261</val></magnitude>
       </node>
       <node name="s__Bacillus_infantis">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Bacillus_weihaiensis">
        <magnitude><val>133</val></magnitude>
       </node>
       <node name="s__Bacillus_halotolerans">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._NEB1478">
        <magnitude><val>73</val></magnitude>
       </node>
       <node name="s__Bacillus_subtilis">
        <magnitude><val>184</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._Cs-700">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._T3">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Bacillus_fonticola">
        <magnitude><val>91</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._KH172YL63">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._1NLA3E">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Bacillus_swezeyi">
        <magnitude><val>110</val></magnitude>
       </node>
       <node name="s__Bacillus_shivajii">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._FJAT-18017">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Bacillus_paralicheniformis">
        <magnitude><val>123</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._THAF10">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Bacillus_luti">
        <magnitude><val>116</val></magnitude>
       </node>
       <node name="s__Bacillus_mycoides">
        <magnitude><val>120</val></magnitude>
       </node>
       <node name="s__Bacillus_vallismortis">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Bacillus_glycinifermentans">
        <magnitude><val>114</val></magnitude>
       </node>
       <node name="s__Bacillus_tropicus">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Bacillus_inaquosorum">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Bacillus_methanolicus">
        <magnitude><val>491</val></magnitude>
       </node>
       <node name="s__Bacillus_cabrialesii">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._DTU_2020_1000418_1_SI_GHA_SEK_038">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Bacillus_pumilus">
        <magnitude><val>114</val></magnitude>
       </node>
       <node name="s__Bacillus_sp._Y1">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Fictibacillus">
       <magnitude><val>533</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fictibacillus_sp._KU28468">
        <magnitude><val>209</val></magnitude>
       </node>
       <node name="s__Fictibacillus_enclensis">
        <magnitude><val>96</val></magnitude>
       </node>
       <node name="s__Fictibacillus_phosphorivorans">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Fictibacillus_arsenicus">
        <magnitude><val>215</val></magnitude>
       </node>
      </node>
      <node name="g__Siminovitchia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>83</val></magnitude>
       <node name="s__Siminovitchia_fortis">
        <magnitude><val>83</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanobacillus">
       <magnitude><val>223</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Oceanobacillus_iheyensis">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Oceanobacillus_zhaokaii">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Oceanobacillus_oncorhynchi">
        <magnitude><val>118</val></magnitude>
       </node>
       <node name="s__Oceanobacillus_kimchii">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Oceanobacillus_jeddahense">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Halalkalibacter">
       <magnitude><val>219</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Halalkalibacter_krulwichiae">
        <magnitude><val>219</val></magnitude>
       </node>
      </node>
      <node name="g__Anoxybacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>640</val></magnitude>
       <node name="s__Anoxybacillus_flavithermus">
        <magnitude><val>538</val></magnitude>
       </node>
       <node name="s__Anoxybacillus_caldiproteolyticus">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Anoxybacillus_gonensis">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Anoxybacillus_amylolyticus">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Gottfriedia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Gottfriedia_acidiceleris">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bacillales_Family_X._Incertae_Sedis">
      <magnitude><val>24</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Hydrogenibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>24</val></magnitude>
       <node name="s__Hydrogenibacillus_sp._N12">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Staphylococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>3957</val></magnitude>
      <node name="g__Jeotgalicoccus">
       <magnitude><val>26</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Jeotgalicoccus_sp._WY2">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Abyssicoccus">
       <magnitude><val>92</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Abyssicoccus_albus">
        <magnitude><val>92</val></magnitude>
       </node>
      </node>
      <node name="g__Staphylococcus">
       <magnitude><val>2648</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Staphylococcus_hyicus">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Staphylococcus_epidermidis">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Staphylococcus_cohnii">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Staphylococcus_lugdunensis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Staphylococcus_arlettae">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Staphylococcus_argenteus">
        <magnitude><val>379</val></magnitude>
       </node>
       <node name="s__Staphylococcus_sp._IVB6227">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Staphylococcus_simiae">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Staphylococcus_felis">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Staphylococcus_edaphicus">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Staphylococcus_rostri">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Staphylococcus_gallinarum">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Staphylococcus_chromogenes">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Staphylococcus_kloosii">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Staphylococcus_pseudoxylosus">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Staphylococcus_haemolyticus">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Staphylococcus_condimenti">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Staphylococcus_nepalensis">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Staphylococcus_succinus">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Staphylococcus_caprae">
        <magnitude><val>69</val></magnitude>
       </node>
       <node name="s__Staphylococcus_aureus">
        <magnitude><val>863</val></magnitude>
       </node>
       <node name="s__Staphylococcus_simulans">
        <magnitude><val>214</val></magnitude>
       </node>
       <node name="s__Staphylococcus_devriesei">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Staphylococcus_auricularis">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Staphylococcus_saprophyticus">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Staphylococcus_piscifermentans">
        <magnitude><val>107</val></magnitude>
       </node>
       <node name="s__Staphylococcus_muscae">
        <magnitude><val>317</val></magnitude>
       </node>
       <node name="s__Staphylococcus_warneri">
        <magnitude><val>121</val></magnitude>
       </node>
       <node name="s__Staphylococcus_pasteuri">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Staphylococcus_pettenkoferi">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Nosocomiicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Nosocomiicoccus_massiliensis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Nosocomiicoccus_ampullae">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Macrococcus">
       <magnitude><val>937</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Macrococcus_equipercicus">
        <magnitude><val>127</val></magnitude>
       </node>
       <node name="s__Macrococcus_bovicus">
        <magnitude><val>126</val></magnitude>
       </node>
       <node name="s__Macrococcus_canis">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Macrococcus_brunensis">
        <magnitude><val>421</val></magnitude>
       </node>
       <node name="s__Macrococcus_epidermidis">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Macrococcus_armenti">
        <magnitude><val>207</val></magnitude>
       </node>
      </node>
      <node name="g__Mammaliicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>192</val></magnitude>
       <node name="s__Mammaliicoccus_stepanovicii">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Mammaliicoccus_vitulinus">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Mammaliicoccus_sciuri">
        <magnitude><val>95</val></magnitude>
       </node>
      </node>
      <node name="g__Salinicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>34</val></magnitude>
       <node name="s__Salinicoccus_halodurans">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sporolactobacillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>210</val></magnitude>
      <node name="g__Sporolactobacillus">
       <magnitude><val>130</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sporolactobacillus_terrae">
        <magnitude><val>130</val></magnitude>
       </node>
      </node>
      <node name="g__Pullulanibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>80</val></magnitude>
       <node name="s__Pullulanibacillus_sp._KACC_23026">
        <magnitude><val>80</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Exiguobacterium">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>373</val></magnitude>
      <node name="s__Exiguobacterium_mexicanum">
       <magnitude><val>38</val></magnitude>
      </node>
      <node name="s__Exiguobacterium_sp._Helios">
       <magnitude><val>135</val></magnitude>
      </node>
      <node name="s__Exiguobacterium_acetylicum">
       <magnitude><val>82</val></magnitude>
      </node>
      <node name="s__Exiguobacterium_sibiricum">
       <magnitude><val>81</val></magnitude>
      </node>
      <node name="s__Exiguobacterium_alkaliphilum">
       <magnitude><val>25</val></magnitude>
      </node>
      <node name="s__Exiguobacterium_sp._N4-1P">
       <magnitude><val>12</val></magnitude>
      </node>
     </node>
     <node name="f__Planococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>2636</val></magnitude>
      <node name="g__Viridibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>115</val></magnitude>
       <node name="s__Viridibacillus_sp._JNUCC-6">
        <magnitude><val>115</val></magnitude>
       </node>
      </node>
      <node name="g__Ureibacillus">
       <magnitude><val>96</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Ureibacillus_thermophilus">
        <magnitude><val>96</val></magnitude>
       </node>
      </node>
      <node name="g__Sporosarcina">
       <magnitude><val>1101</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sporosarcina_sp._Te-1">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Sporosarcina_sp._Marseille-Q4943">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Sporosarcina_sp._PTS2304">
        <magnitude><val>631</val></magnitude>
       </node>
       <node name="s__Sporosarcina_pasteurii">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Sporosarcina_sp._T2O-4">
        <magnitude><val>93</val></magnitude>
       </node>
       <node name="s__Sporosarcina_sp._0.2-SM1T-5">
        <magnitude><val>118</val></magnitude>
       </node>
       <node name="s__Sporosarcina_ureae">
        <magnitude><val>134</val></magnitude>
       </node>
       <node name="s__Sporosarcina_ureilytica">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Sporosarcina_thermotolerans">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Solibacillus">
       <magnitude><val>200</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Solibacillus_daqui">
        <magnitude><val>200</val></magnitude>
       </node>
      </node>
      <node name="g__Paenisporosarcina">
       <magnitude><val>21</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paenisporosarcina_antarctica">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Planococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>995</val></magnitude>
       <node name="s__Planococcus_halotolerans">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Planococcus_faecalis">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Planococcus_maritimus">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Planococcus_sp._N022">
        <magnitude><val>323</val></magnitude>
       </node>
       <node name="s__Planococcus_lenghuensis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Planococcus_massiliensis">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Planococcus_glaciei">
        <magnitude><val>395</val></magnitude>
       </node>
       <node name="s__Planococcus_halocryophilus">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Planococcus_sp._N016">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Planococcus_antarcticus">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Jeotgalibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>108</val></magnitude>
       <node name="s__Jeotgalibacillus_malaysiensis">
        <magnitude><val>108</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Alicyclobacillaceae">
      <magnitude><val>625</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Alicyclobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>573</val></magnitude>
       <node name="s__Alicyclobacillus_acidocaldarius">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Alicyclobacillus_mengziensis">
        <magnitude><val>465</val></magnitude>
       </node>
       <node name="s__Alicyclobacillus_cycloheptanicus">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Alicyclobacillus_acidoterrestris">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Alicyclobacillus_fastidiosus">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Alicyclobacillus_sp._ALC3">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Effusibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Effusibacillus_dendaii">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Tumebacillus">
       <magnitude><val>33</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tumebacillus_avium">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermoactinomycetaceae">
      <magnitude><val>246</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Novibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Novibacillus_thermophilus">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Laceyella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Laceyella_sacchari">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Staphylospora">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Staphylospora_marina">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Thermoactinomyces">
       <magnitude><val>137</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermoactinomyces_vulgaris">
        <magnitude><val>137</val></magnitude>
       </node>
      </node>
      <node name="g__Kroppenstedtia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Kroppenstedtia_eburnea">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Polycladomyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Polycladomyces_abyssicola">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Listeriaceae">
      <magnitude><val>2025</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Listeria">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1985</val></magnitude>
       <node name="s__Listeria_welshimeri">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Listeria_monocytogenes">
        <magnitude><val>967</val></magnitude>
       </node>
       <node name="s__Listeria_sp._PSOL-1">
        <magnitude><val>65</val></magnitude>
       </node>
       <node name="s__Listeria_marthii">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Listeria_newyorkensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Listeria_weihenstephanensis">
        <magnitude><val>388</val></magnitude>
       </node>
       <node name="s__Listeria_grayi">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Listeria_innocua">
        <magnitude><val>479</val></magnitude>
       </node>
      </node>
      <node name="g__Brochothrix">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>40</val></magnitude>
       <node name="s__Brochothrix_thermosphacta">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Paenibacillaceae">
      <magnitude><val>12432</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Saccharibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>100</val></magnitude>
       <node name="s__Saccharibacillus_brassicae">
        <magnitude><val>100</val></magnitude>
       </node>
      </node>
      <node name="g__Paenibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10671</val></magnitude>
       <node name="s__Paenibacillus_stellifer">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Paenibacillus_jilunlii">
        <magnitude><val>130</val></magnitude>
       </node>
       <node name="s__Paenibacillus_azoreducens">
        <magnitude><val>153</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._JNUCC-31">
        <magnitude><val>338</val></magnitude>
       </node>
       <node name="s__Paenibacillus_physcomitrellae">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._H1-7">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sabinae">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sonchi">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._FSL_R7-0331">
        <magnitude><val>92</val></magnitude>
       </node>
       <node name="s__Paenibacillus_woosongensis">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Paenibacillus_cellulosilyticus">
        <magnitude><val>190</val></magnitude>
       </node>
       <node name="s__Paenibacillus_borealis">
        <magnitude><val>173</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._Cedars">
        <magnitude><val>176</val></magnitude>
       </node>
       <node name="s__Paenibacillus_montanisoli">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Paenibacillus_xylanexedens">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._19GGS1-52">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._BIHB_4019">
        <magnitude><val>93</val></magnitude>
       </node>
       <node name="s__Paenibacillus_konkukensis">
        <magnitude><val>133</val></magnitude>
       </node>
       <node name="s__Paenibacillus_alvei">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sophorae">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Paenibacillus_ihbetae">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._JZ16">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._E222">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Paenibacillus_brasilensis">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._32O-W">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._DCT19">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Paenibacillus_yonginensis">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._C31">
        <magnitude><val>135</val></magnitude>
       </node>
       <node name="s__Paenibacillus_uliginis">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Paenibacillus_tritici">
        <magnitude><val>115</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._BR1-192">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._FSL_H7-0737">
        <magnitude><val>121</val></magnitude>
       </node>
       <node name="s__Paenibacillus_andongensis">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._YPG26">
        <magnitude><val>63</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._sptzw28">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._RUD330">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._IHB_B_3084">
        <magnitude><val>87</val></magnitude>
       </node>
       <node name="s__Paenibacillus_lycopersici">
        <magnitude><val>100</val></magnitude>
       </node>
       <node name="s__Paenibacillus_elgii">
        <magnitude><val>292</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._IHBB_10380">
        <magnitude><val>94</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._D2_2">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._FSL_R5-0345">
        <magnitude><val>331</val></magnitude>
       </node>
       <node name="s__Paenibacillus_rhizovicinus">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._MBLB1832">
        <magnitude><val>76</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._URB8-2">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Paenibacillus_xylanilyticus">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._HWE-109">
        <magnitude><val>81</val></magnitude>
       </node>
       <node name="s__Paenibacillus_baekrokdamisoli">
        <magnitude><val>156</val></magnitude>
       </node>
       <node name="s__Paenibacillus_albicereus">
        <magnitude><val>94</val></magnitude>
       </node>
       <node name="s__Paenibacillus_swuensis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Paenibacillus_thiaminolyticus">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._PAMC21692">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Paenibacillus_barcinonensis">
        <magnitude><val>126</val></magnitude>
       </node>
       <node name="s__Paenibacillus_durus">
        <magnitude><val>103</val></magnitude>
       </node>
       <node name="s__Paenibacillus_odorifer">
        <magnitude><val>157</val></magnitude>
       </node>
       <node name="s__Paenibacillus_riograndensis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._JDR-2">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._B01">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Paenibacillus_pabuli">
        <magnitude><val>152</val></magnitude>
       </node>
       <node name="s__Paenibacillus_protaetiae">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._FSL_H7-0357">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Paenibacillus_mucilaginosus">
        <magnitude><val>226</val></magnitude>
       </node>
       <node name="s__Paenibacillus_glucanolyticus">
        <magnitude><val>396</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._BIC5C1">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._G2S3">
        <magnitude><val>73</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._SYP-B4298">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._CAA11">
        <magnitude><val>223</val></magnitude>
       </node>
       <node name="s__Paenibacillus_kribbensis">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Paenibacillus_chitinolyticus">
        <magnitude><val>76</val></magnitude>
       </node>
       <node name="s__Paenibacillus_macerans">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._481">
        <magnitude><val>110</val></magnitude>
       </node>
       <node name="s__Paenibacillus_donghaensis">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._PSB04">
        <magnitude><val>485</val></magnitude>
       </node>
       <node name="s__Paenibacillus_beijingensis">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Paenibacillus_dendritiformis">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Paenibacillus_naphthalenovorans">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Paenibacillus_typhae">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Paenibacillus_lutimineralis">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._MBLB1776">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Paenibacillus_algicola">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Paenibacillus_psychroresistens">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._RC67">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._R14(2021)">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Paenibacillus_guangzhouensis">
        <magnitude><val>1015</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._MMS20-IR301">
        <magnitude><val>124</val></magnitude>
       </node>
       <node name="s__Paenibacillus_spongiae">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Paenibacillus_amylolyticus">
        <magnitude><val>162</val></magnitude>
       </node>
       <node name="s__Paenibacillus_bovis">
        <magnitude><val>91</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._YPD9-1">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Paenibacillus_polymyxa">
        <magnitude><val>1030</val></magnitude>
       </node>
       <node name="s__Paenibacillus_larvae">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Paenibacillus_urinalis">
        <magnitude><val>138</val></magnitude>
       </node>
       <node name="s__Paenibacillus_marchantiae">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Paenibacillus_antarcticus">
        <magnitude><val>108</val></magnitude>
       </node>
       <node name="s__Paenibacillus_sp._PK3_47">
        <magnitude><val>131</val></magnitude>
       </node>
       <node name="s__Paenibacillus_tianjinensis">
        <magnitude><val>276</val></magnitude>
       </node>
       <node name="s__Paenibacillus_graminis">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Cohnella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>87</val></magnitude>
       <node name="s__Cohnella_candidum">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Cohnella_sp._LGH">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Cohnella_cholangitidis">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Cohnella_abietis">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Aneurinibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>143</val></magnitude>
       <node name="s__Aneurinibacillus_sp._Ricciae_BoGa-3">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Aneurinibacillus_sp._B1">
        <magnitude><val>92</val></magnitude>
       </node>
      </node>
      <node name="g__Thermobacillus">
       <magnitude><val>48</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermobacillus_composti">
        <magnitude><val>48</val></magnitude>
       </node>
      </node>
      <node name="g__Brevibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1383</val></magnitude>
       <node name="s__Brevibacillus_borstelensis">
        <magnitude><val>258</val></magnitude>
       </node>
       <node name="s__Brevibacillus_humidisoli">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Brevibacillus_choshinensis">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Brevibacillus_brevis">
        <magnitude><val>293</val></magnitude>
       </node>
       <node name="s__Brevibacillus_sp._JNUCC-41">
        <magnitude><val>188</val></magnitude>
       </node>
       <node name="s__Brevibacillus_laterosporus">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Brevibacillus_composti">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Brevibacillus_sp._WF146">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Brevibacillus_sp._BB3-R1">
        <magnitude><val>396</val></magnitude>
       </node>
       <node name="s__Brevibacillus_agri">
        <magnitude><val>108</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Negativicutes">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>531677</val></magnitude>
    <node name="o__Selenomonadales">
     <magnitude><val>2918</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Selenomonadaceae">
      <magnitude><val>1940</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Selenomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1491</val></magnitude>
       <node name="s__Selenomonas_sp._oral_taxon_136">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Selenomonas_timonae">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Selenomonas_sp._oral_taxon_920">
        <magnitude><val>184</val></magnitude>
       </node>
       <node name="s__Selenomonas_ruminantium">
        <magnitude><val>96</val></magnitude>
       </node>
       <node name="s__Selenomonas_sputigena">
        <magnitude><val>663</val></magnitude>
       </node>
       <node name="s__Selenomonas_sp._oral_taxon_478">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Selenomonas_dianae">
        <magnitude><val>449</val></magnitude>
       </node>
      </node>
      <node name="g__Megamonas">
       <magnitude><val>353</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Megamonas_funiformis">
        <magnitude><val>275</val></magnitude>
       </node>
       <node name="s__Megamonas_hypermegale">
        <magnitude><val>78</val></magnitude>
       </node>
      </node>
      <node name="g__Selenobaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>74</val></magnitude>
       <node name="s__Selenobaculum_gbiensis">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
      <node name="g__Pectinatus">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pectinatus_frisingensis">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sporomusaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>978</val></magnitude>
      <node name="g__Anaeromusa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__uncultured_Anaeromusa_sp.">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Sporomusa">
       <magnitude><val>241</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sporomusa_termitida">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__uncultured_Sporomusa_sp.">
        <magnitude><val>211</val></magnitude>
       </node>
      </node>
      <node name="g__Methylomusa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>320</val></magnitude>
       <node name="s__Methylomusa_anaerophila">
        <magnitude><val>320</val></magnitude>
       </node>
      </node>
      <node name="g__Pelosinus">
       <magnitude><val>384</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pelosinus_sp._UFO1">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Pelosinus_fermentans">
        <magnitude><val>344</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Acidaminococcales">
     <magnitude><val>526226</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Acidaminococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>526226</val></magnitude>
      <node name="g__Phascolarctobacterium">
       <magnitude><val>379081</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Phascolarctobacterium_faecium">
        <magnitude><val>378590</val></magnitude>
       </node>
       <node name="s__Phascolarctobacterium_succinatutens">
        <magnitude><val>217</val></magnitude>
       </node>
       <node name="s__Phascolarctobacterium_sp._Marseille-Q4147">
        <magnitude><val>274</val></magnitude>
       </node>
      </node>
      <node name="g__Acidaminococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>147145</val></magnitude>
       <node name="s__Acidaminococcus_intestini">
        <magnitude><val>147005</val></magnitude>
       </node>
       <node name="s__Acidaminococcus_fermentans">
        <magnitude><val>140</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Veillonellales">
     <magnitude><val>2533</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Veillonellaceae">
      <magnitude><val>2533</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Megasphaera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1867</val></magnitude>
       <node name="s__Megasphaera_hexanoica">
        <magnitude><val>826</val></magnitude>
       </node>
       <node name="s__Megasphaera_massiliensis">
        <magnitude><val>127</val></magnitude>
       </node>
       <node name="s__Megasphaera_stantonii">
        <magnitude><val>457</val></magnitude>
       </node>
       <node name="s__Megasphaera_elsdenii">
        <magnitude><val>457</val></magnitude>
       </node>
      </node>
      <node name="g__Veillonella">
       <magnitude><val>415</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Veillonella_atypica">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Veillonella_rogosae">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Veillonella_rodentium">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Veillonella_parvula">
        <magnitude><val>116</val></magnitude>
       </node>
       <node name="s__Veillonella_sp._S12025-13">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Veillonella_dispar">
        <magnitude><val>116</val></magnitude>
       </node>
      </node>
      <node name="g__Dialister">
       <magnitude><val>251</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dialister_succinatiphilus">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Dialister_massiliensis">
        <magnitude><val>152</val></magnitude>
       </node>
       <node name="s__Dialister_pneumosintes">
        <magnitude><val>56</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Limnochordia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>16</val></magnitude>
    <node name="o__Limnochordales">
     <magnitude><val>16</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Limnochordaceae">
      <magnitude><val>16</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Limnochorda">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Limnochorda_pilosa">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Clostridia">
    <magnitude><val>13520249</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Halanaerobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>741</val></magnitude>
     <node name="f__Halothermotrichaceae">
      <magnitude><val>60</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Halothermothrix">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>60</val></magnitude>
       <node name="s__Halothermothrix_orenii">
        <magnitude><val>60</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Halanaerobiaceae">
      <magnitude><val>234</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Halanaerobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>234</val></magnitude>
       <node name="s__Halanaerobium_praevalens">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Halanaerobium_hydrogeniformans">
        <magnitude><val>170</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Halobacteroidaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>32</val></magnitude>
      <node name="g__Halobacteroides">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Halobacteroides_halobius">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Acetohalobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Acetohalobium_arabaticum">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Anoxybacter">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>415</val></magnitude>
      <node name="s__Anoxybacter_fermentans">
       <magnitude><val>415</val></magnitude>
      </node>
     </node>
    </node>
    <node name="o__Thermoanaerobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1462</val></magnitude>
     <node name="f__Thermoanaerobacterales_Family_IV._Incertae_Sedis">
      <magnitude><val>29</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Mahella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Mahella_australiensis">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermoanaerobacteraceae">
      <magnitude><val>1393</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermoanaerobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>456</val></magnitude>
       <node name="s__Thermoanaerobacter_kivui">
        <magnitude><val>456</val></magnitude>
       </node>
      </node>
      <node name="g__Thermoanaerobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>339</val></magnitude>
       <node name="s__Thermoanaerobacterium_sp._RBIITD">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Thermoanaerobacterium_thermosaccharolyticum">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Thermoanaerobacterium_sp._CMT5567-10">
        <magnitude><val>265</val></magnitude>
       </node>
      </node>
      <node name="g__Caldanaerobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27</val></magnitude>
       <node name="s__Caldanaerobacter_subterraneus">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Ammonifex">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>260</val></magnitude>
       <node name="s__Ammonifex_degensii">
        <magnitude><val>260</val></magnitude>
       </node>
      </node>
      <node name="g__Carboxydothermus">
       <magnitude><val>41</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Carboxydothermus_hydrogenoformans">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Gelria">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Gelria_sp._Kuro-4">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Thermacetogenium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>58</val></magnitude>
       <node name="s__Thermacetogenium_phaeum">
        <magnitude><val>58</val></magnitude>
       </node>
      </node>
      <node name="g__Aceticella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>189</val></magnitude>
       <node name="s__Aceticella_autotrophica">
        <magnitude><val>189</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermodesulfobiaceae">
      <magnitude><val>40</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermodesulfobium">
       <magnitude><val>40</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermodesulfobium_acidiphilum">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Thermodesulfobium_narugense">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Natranaerobiales">
     <magnitude><val>91</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Natranaerobiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>91</val></magnitude>
      <node name="g__Natranaerobius">
       <magnitude><val>91</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Natranaerobius_thermophilus">
        <magnitude><val>91</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Moorellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>243</val></magnitude>
     <node name="f__Moorellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>129</val></magnitude>
      <node name="g__Moorella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>129</val></magnitude>
       <node name="s__Moorella_sp._Hama-1">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Moorella_glycerini">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Moorella_thermoacetica">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Zhaonellaceae">
      <magnitude><val>114</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Zhaonella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>114</val></magnitude>
       <node name="s__Zhaonella_formicivorans">
        <magnitude><val>114</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Thermosediminibacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>70</val></magnitude>
     <node name="f__Thermosediminibacteraceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermosediminibacter">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermosediminibacter_oceani">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Tepidanaerobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>59</val></magnitude>
      <node name="g__Tepidanaerobacter">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tepidanaerobacter_acetatoxydans">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Biomaibacter">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Biomaibacter_acetigenes">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Koleobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>157</val></magnitude>
     <node name="f__Koleobacteraceae">
      <magnitude><val>157</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Koleobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>157</val></magnitude>
       <node name="s__Koleobacter_methoxysyntrophicus">
        <magnitude><val>157</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Eubacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>13515158</val></magnitude>
     <node name="g__Fenollaria">
      <magnitude><val>54</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Fenollaria_massiliensis">
       <magnitude><val>30</val></magnitude>
      </node>
      <node name="s__Fenollaria_sporofastidiosus">
       <magnitude><val>24</val></magnitude>
      </node>
     </node>
     <node name="f__Cellulosilyticaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>302</val></magnitude>
      <node name="g__Cellulosilyticum">
       <magnitude><val>302</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cellulosilyticum_sp._WCF-2">
        <magnitude><val>189</val></magnitude>
       </node>
       <node name="s__Cellulosilyticum_lentocellum">
        <magnitude><val>113</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfitobacteriaceae">
      <magnitude><val>2912</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Syntrophobotulus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>462</val></magnitude>
       <node name="s__Syntrophobotulus_glycolicus">
        <magnitude><val>462</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfosporosinus">
       <magnitude><val>1688</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfosporosinus_acidiphilus">
        <magnitude><val>253</val></magnitude>
       </node>
       <node name="s__Desulfosporosinus_youngiae">
        <magnitude><val>529</val></magnitude>
       </node>
       <node name="s__Desulfosporosinus_meridiei">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__Desulfosporosinus_orientis">
        <magnitude><val>871</val></magnitude>
       </node>
      </node>
      <node name="g__Dehalobacter">
       <magnitude><val>101</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dehalobacter_restrictus">
        <magnitude><val>101</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfitobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>661</val></magnitude>
       <node name="s__Desulfitobacterium_dehalogenans">
        <magnitude><val>82</val></magnitude>
       </node>
       <node name="s__Desulfitobacterium_metallireducens">
        <magnitude><val>148</val></magnitude>
       </node>
       <node name="s__Desulfitobacterium_dichloroeliminans">
        <magnitude><val>169</val></magnitude>
       </node>
       <node name="s__Desulfitobacterium_hafniense">
        <magnitude><val>262</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Clostridiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>78514</val></magnitude>
      <node name="g__Hungatella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>45217</val></magnitude>
       <node name="s__Hungatella_hathewayi">
        <magnitude><val>43131</val></magnitude>
       </node>
       <node name="s__Hungatella_xylanolytica">
        <magnitude><val>2086</val></magnitude>
       </node>
      </node>
      <node name="g__Paraclostridium">
       <magnitude><val>169</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paraclostridium_bifermentans">
        <magnitude><val>169</val></magnitude>
       </node>
      </node>
      <node name="g__Clostridium">
       <magnitude><val>30700</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Clostridium_formicaceticum">
        <magnitude><val>125</val></magnitude>
       </node>
       <node name="s__Clostridium_manihotivorum">
        <magnitude><val>128</val></magnitude>
       </node>
       <node name="s__Clostridium_gasigenes">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Clostridium_pasteurianum">
        <magnitude><val>205</val></magnitude>
       </node>
       <node name="s__Clostridium_novyi">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Clostridium_estertheticum">
        <magnitude><val>338</val></magnitude>
       </node>
       <node name="s__Clostridium_fermenticellae">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Clostridium_beijerinckii">
        <magnitude><val>347</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._MB40-C1">
        <magnitude><val>132</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._'deep_sea'">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Clostridium_gelidum">
        <magnitude><val>174</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._BJN0001">
        <magnitude><val>168</val></magnitude>
       </node>
       <node name="s__Clostridium_botulinum">
        <magnitude><val>736</val></magnitude>
       </node>
       <node name="s__Clostridium_septicum">
        <magnitude><val>244</val></magnitude>
       </node>
       <node name="s__Clostridium_acetobutylicum">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Clostridium_thermarum">
        <magnitude><val>223</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._DL-VIII">
        <magnitude><val>379</val></magnitude>
       </node>
       <node name="s__Clostridium_cochlearium">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._M62/1">
        <magnitude><val>12778</val></magnitude>
       </node>
       <node name="s__Clostridium_aceticum">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._MD294">
        <magnitude><val>1116</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._001">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Clostridium_butyricum">
        <magnitude><val>140</val></magnitude>
       </node>
       <node name="s__Clostridium_tagluense">
        <magnitude><val>105</val></magnitude>
       </node>
       <node name="s__Clostridium_chauvoei">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Clostridium_saccharobutylicum">
        <magnitude><val>190</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._CF011">
        <magnitude><val>167</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._OS1-26">
        <magnitude><val>236</val></magnitude>
       </node>
       <node name="s__Clostridium_intestinale">
        <magnitude><val>194</val></magnitude>
       </node>
       <node name="s__Clostridium_drakei">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._C1">
        <magnitude><val>541</val></magnitude>
       </node>
       <node name="s__Clostridium_tyrobutyricum">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Clostridium_kluyveri">
        <magnitude><val>412</val></magnitude>
       </node>
       <node name="s__Clostridium_cadaveris">
        <magnitude><val>1143</val></magnitude>
       </node>
       <node name="s__Clostridium_sporogenes">
        <magnitude><val>873</val></magnitude>
       </node>
       <node name="s__Clostridium_taeniosporum">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Clostridium_baratii">
        <magnitude><val>505</val></magnitude>
       </node>
       <node name="s__Clostridium_scatologenes">
        <magnitude><val>127</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._BNL1100">
        <magnitude><val>526</val></magnitude>
       </node>
       <node name="s__Clostridium_tetani">
        <magnitude><val>173</val></magnitude>
       </node>
       <node name="s__Clostridium_isatidis">
        <magnitude><val>186</val></magnitude>
       </node>
       <node name="s__Clostridium_perfringens">
        <magnitude><val>3079</val></magnitude>
       </node>
       <node name="s__Clostridium_cellulovorans">
        <magnitude><val>121</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._LQ25">
        <magnitude><val>451</val></magnitude>
       </node>
       <node name="s__Clostridium_bornimense">
        <magnitude><val>151</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._JN-9">
        <magnitude><val>122</val></magnitude>
       </node>
       <node name="s__Clostridium_saccharoperbutylacetonicum">
        <magnitude><val>177</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._JN-1">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Clostridium_carboxidivorans">
        <magnitude><val>146</val></magnitude>
       </node>
       <node name="s__Clostridium_felsineum">
        <magnitude><val>118</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._JS66">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Clostridium_argentinense">
        <magnitude><val>165</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._AWRP">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Clostridium_sp._SY8519">
        <magnitude><val>2839</val></magnitude>
       </node>
      </node>
      <node name="g__Proteiniclasticum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>173</val></magnitude>
       <node name="s__Proteiniclasticum_sp._QWL-01">
        <magnitude><val>173</val></magnitude>
       </node>
      </node>
      <node name="g__Crassaminicella">
       <magnitude><val>332</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Crassaminicella_thermophila">
        <magnitude><val>93</val></magnitude>
       </node>
       <node name="s__Crassaminicella_profunda">
        <magnitude><val>121</val></magnitude>
       </node>
       <node name="s__Crassaminicella_indica">
        <magnitude><val>118</val></magnitude>
       </node>
      </node>
      <node name="g__Alkaliphilus">
       <magnitude><val>287</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Alkaliphilus_oremlandii">
        <magnitude><val>125</val></magnitude>
       </node>
       <node name="s__Alkaliphilus_sp._B6464">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Alkaliphilus_metalliredigens">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
      <node name="g__Caminicella">
       <magnitude><val>535</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caminicella_sporogenes">
        <magnitude><val>535</val></magnitude>
       </node>
      </node>
      <node name="g__Geosporobacter">
       <magnitude><val>165</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Geosporobacter_ferrireducens">
        <magnitude><val>165</val></magnitude>
       </node>
      </node>
      <node name="g__Hathewaya">
       <magnitude><val>35</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Hathewaya_histolytica">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Arthromitus">
       <magnitude><val>42</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Arthromitus_sp._SFB-rat-Yit">
        <magnitude><val>42</val></magnitude>
       </node>
      </node>
      <node name="g__Serpentinicella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>43</val></magnitude>
       <node name="s__Serpentinicella_alkaliphila">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
      <node name="g__Caloramator">
       <magnitude><val>668</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caloramator_sp._mosi_1">
        <magnitude><val>153</val></magnitude>
       </node>
       <node name="s__Caloramator_sp._E03">
        <magnitude><val>417</val></magnitude>
       </node>
       <node name="s__Caloramator_sp._Dgby_cultured_2">
        <magnitude><val>98</val></magnitude>
       </node>
      </node>
      <node name="g__Sarcina">
       <magnitude><val>40</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sarcina_sp._JB2">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanirhabdus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>108</val></magnitude>
       <node name="s__Oceanirhabdus_sp._W0125-5">
        <magnitude><val>108</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermincolaceae">
      <magnitude><val>23</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermincola">
       <magnitude><val>23</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermincola_potens">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Oscillospiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>933104</val></magnitude>
      <node name="g__Ethanoligenens">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2884</val></magnitude>
       <node name="s__Ethanoligenens_harbinense">
        <magnitude><val>2884</val></magnitude>
       </node>
      </node>
      <node name="g__Ruminiclostridium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1348</val></magnitude>
       <node name="s__Ruminiclostridium_cellulolyticum">
        <magnitude><val>190</val></magnitude>
       </node>
       <node name="s__Ruminiclostridium_herbifermentans">
        <magnitude><val>298</val></magnitude>
       </node>
       <node name="s__Ruminiclostridium_papyrosolvens">
        <magnitude><val>860</val></magnitude>
       </node>
      </node>
      <node name="g__Ruminococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>378008</val></magnitude>
       <node name="s__Ruminococcus_sp._SR1/5">
        <magnitude><val>37346</val></magnitude>
       </node>
       <node name="s__Ruminococcus_gauvreauii">
        <magnitude><val>3848</val></magnitude>
       </node>
       <node name="s__Ruminococcus_bovis">
        <magnitude><val>23234</val></magnitude>
       </node>
       <node name="s__Ruminococcus_champanellensis">
        <magnitude><val>4392</val></magnitude>
       </node>
       <node name="s__Ruminococcus_albus">
        <magnitude><val>3574</val></magnitude>
       </node>
       <node name="s__Ruminococcus_bicirculans_(ex_Wegman_et_al._2014)">
        <magnitude><val>11540</val></magnitude>
       </node>
       <node name="s__Ruminococcus_sp._FMB-CY1">
        <magnitude><val>294074</val></magnitude>
       </node>
      </node>
      <node name="g__Acutalibacter">
       <magnitude><val>2747</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Acutalibacter_muris">
        <magnitude><val>2747</val></magnitude>
       </node>
      </node>
      <node name="g__Lawsonibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17695</val></magnitude>
       <node name="s__Lawsonibacter_asaccharolyticus">
        <magnitude><val>17695</val></magnitude>
       </node>
      </node>
      <node name="g__Subdoligranulum">
       <magnitude><val>3244</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Subdoligranulum_variabile">
        <magnitude><val>3244</val></magnitude>
       </node>
      </node>
      <node name="g__Faecalibacterium">
       <magnitude><val>158481</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Faecalibacterium_sp._IP-1-18">
        <magnitude><val>16069</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._I3-3-33">
        <magnitude><val>3868</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._I4-3-84">
        <magnitude><val>17501</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_duncaniae">
        <magnitude><val>23402</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._IP-3-29">
        <magnitude><val>10377</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._I4-1-79">
        <magnitude><val>3795</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._I3-3-89">
        <magnitude><val>8213</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_prausnitzii">
        <magnitude><val>67993</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._HTF-F">
        <magnitude><val>5436</val></magnitude>
       </node>
       <node name="s__Faecalibacterium_sp._I2-3-92">
        <magnitude><val>1827</val></magnitude>
       </node>
      </node>
      <node name="g__Monoglobus">
       <magnitude><val>15944</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Monoglobus_pectinilyticus">
        <magnitude><val>15944</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudoclostridium">
       <magnitude><val>438</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudoclostridium_thermosuccinogenes">
        <magnitude><val>438</val></magnitude>
       </node>
      </node>
      <node name="g__Caproicibacterium">
       <magnitude><val>6813</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caproicibacterium_sp._BJN0003">
        <magnitude><val>2753</val></magnitude>
       </node>
       <node name="s__Caproicibacterium_amylolyticum">
        <magnitude><val>580</val></magnitude>
       </node>
       <node name="s__Caproicibacterium_lactatifermentans">
        <magnitude><val>2412</val></magnitude>
       </node>
       <node name="s__Caproicibacterium_sp._ZCY20-5">
        <magnitude><val>1068</val></magnitude>
       </node>
      </node>
      <node name="g__Oscillibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2202</val></magnitude>
       <node name="s__Oscillibacter_hominis">
        <magnitude><val>2202</val></magnitude>
       </node>
      </node>
      <node name="g__Caproiciproducens">
       <magnitude><val>1671</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caproiciproducens_sp._NJN-50">
        <magnitude><val>481</val></magnitude>
       </node>
       <node name="s__uncultured_Caproiciproducens_sp.">
        <magnitude><val>1190</val></magnitude>
       </node>
      </node>
      <node name="g__Dysosmobacter">
       <magnitude><val>33928</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dysosmobacter_welbionis">
        <magnitude><val>33928</val></magnitude>
       </node>
      </node>
      <node name="g__Pusillibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>6301</val></magnitude>
       <node name="s__Pusillibacter_faecalis">
        <magnitude><val>6301</val></magnitude>
       </node>
      </node>
      <node name="g__Paludihabitans">
       <magnitude><val>1229</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paludicola_sp._MB14-C6">
        <magnitude><val>1229</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerotruncus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16716</val></magnitude>
       <node name="s__Anaerotruncus_colihominis">
        <magnitude><val>16716</val></magnitude>
       </node>
      </node>
      <node name="g__Fastidiosipila">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>162</val></magnitude>
       <node name="s__Fastidiosipila_sanguinis">
        <magnitude><val>162</val></magnitude>
       </node>
      </node>
      <node name="g__Caproicibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1028</val></magnitude>
       <node name="s__Caproicibacter_fermentans">
        <magnitude><val>1028</val></magnitude>
       </node>
      </node>
      <node name="g__Thermoclostridium">
       <magnitude><val>328</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermoclostridium_stercorarium">
        <magnitude><val>328</val></magnitude>
       </node>
      </node>
      <node name="g__Petroclostridium">
       <magnitude><val>576</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Petroclostridium_sp._X23">
        <magnitude><val>576</val></magnitude>
       </node>
      </node>
      <node name="g__Acetivibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>998</val></magnitude>
       <node name="s__Acetivibrio_clariflavus">
        <magnitude><val>373</val></magnitude>
       </node>
       <node name="s__Acetivibrio_thermocellus">
        <magnitude><val>329</val></magnitude>
       </node>
       <node name="s__Acetivibrio_saccincola">
        <magnitude><val>296</val></magnitude>
       </node>
      </node>
      <node name="g__Mageeibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>176</val></magnitude>
       <node name="s__Mageeibacillus_indolicus">
        <magnitude><val>176</val></magnitude>
       </node>
      </node>
      <node name="g__Ruthenibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>187875</val></magnitude>
       <node name="s__Ruthenibacterium_lactatiformans">
        <magnitude><val>187875</val></magnitude>
       </node>
      </node>
      <node name="g__Solibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12059</val></magnitude>
       <node name="s__Solibaculum_mannosilyticum">
        <magnitude><val>12059</val></magnitude>
       </node>
      </node>
      <node name="g__Vescimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>5984</val></magnitude>
       <node name="s__Vescimonas_fastidiosa">
        <magnitude><val>3493</val></magnitude>
       </node>
       <node name="s__Vescimonas_coprocola">
        <magnitude><val>2491</val></magnitude>
       </node>
      </node>
      <node name="g__Agathobaculum">
       <magnitude><val>1638</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Agathobaculum_sp._NTUH-O15-33">
        <magnitude><val>1638</val></magnitude>
       </node>
      </node>
      <node name="g__Flavonifractor">
       <magnitude><val>71603</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Flavonifractor_plautii">
        <magnitude><val>71603</val></magnitude>
       </node>
      </node>
      <node name="g__Amygdalobacter">
       <magnitude><val>308</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Amygdalobacter_nucleatus">
        <magnitude><val>204</val></magnitude>
       </node>
       <node name="s__Amygdalobacter_indicium">
        <magnitude><val>104</val></magnitude>
       </node>
      </node>
      <node name="g__Thermocaproicibacter">
       <magnitude><val>720</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermocaproicibacter_melissae">
        <magnitude><val>720</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfallaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>17</val></magnitude>
      <node name="g__Desulfoscipio">
       <magnitude><val>17</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfoscipio_gibsoniae">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Massilistercora">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>23183</val></magnitude>
      <node name="s__Massilistercora_timonensis">
       <magnitude><val>23183</val></magnitude>
      </node>
     </node>
     <node name="f__Syntrophomonadaceae">
      <magnitude><val>42</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Syntrophocurvum">
       <magnitude><val>21</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Syntrophocurvum_alkaliphilum">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Syntrophomonas">
       <magnitude><val>21</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Syntrophomonas_wolfei">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Clostridiales_Family_XVII._Incertae_Sedis">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>62</val></magnitude>
      <node name="g__Thermaerobacter">
       <magnitude><val>62</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermaerobacter_sp._PB12/4term">
        <magnitude><val>62</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Christensenellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>603</val></magnitude>
      <node name="g__Christensenella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>603</val></magnitude>
       <node name="s__Christensenella_minuta">
        <magnitude><val>603</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Lachnospiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>12314933</val></magnitude>
      <node name="g__Marvinbryantia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>183852</val></magnitude>
       <node name="s__Marvinbryantia_formatexigens">
        <magnitude><val>183852</val></magnitude>
       </node>
      </node>
      <node name="g__Agathobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2576919</val></magnitude>
       <node name="s__Agathobacter_rectalis">
        <magnitude><val>2576919</val></magnitude>
       </node>
      </node>
      <node name="g__Lachnoanaerobaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>5485</val></magnitude>
       <node name="s__Lachnoanaerobaculum_umeaense">
        <magnitude><val>1698</val></magnitude>
       </node>
       <node name="s__Lachnoanaerobaculum_gingivalis">
        <magnitude><val>3787</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudobutyrivibrio">
       <magnitude><val>2541</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudobutyrivibrio_xylanivorans">
        <magnitude><val>2541</val></magnitude>
       </node>
      </node>
      <node name="g__Novisyntrophococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>4357</val></magnitude>
       <node name="s__Novisyntrophococcus_fermenticellae">
        <magnitude><val>4357</val></magnitude>
       </node>
      </node>
      <node name="g__Chordicoccus">
       <magnitude><val>932</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Chordicoccus_furentiruminis">
        <magnitude><val>932</val></magnitude>
       </node>
      </node>
      <node name="g__Lacrimispora">
       <magnitude><val>11577</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lacrimispora_xylanolytica">
        <magnitude><val>3659</val></magnitude>
       </node>
       <node name="s__Lacrimispora_saccharolytica">
        <magnitude><val>3654</val></magnitude>
       </node>
       <node name="s__Lacrimispora_sphenoides">
        <magnitude><val>4264</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerotignum">
       <magnitude><val>2332</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaerotignum_propionicum">
        <magnitude><val>1135</val></magnitude>
       </node>
       <node name="s__Anaerotignum_sp._MB30-C6">
        <magnitude><val>1197</val></magnitude>
       </node>
      </node>
      <node name="g__Coprococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>328551</val></magnitude>
       <node name="s__Coprococcus_sp._ART55/1">
        <magnitude><val>18219</val></magnitude>
       </node>
       <node name="s__Coprococcus_catus">
        <magnitude><val>33202</val></magnitude>
       </node>
       <node name="s__Coprococcus_eutactus">
        <magnitude><val>13940</val></magnitude>
       </node>
       <node name="s__Coprococcus_comes">
        <magnitude><val>263190</val></magnitude>
       </node>
      </node>
      <node name="g__Anaeropeptidivorans">
       <magnitude><val>1081</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaeropeptidivorans_aminofermentans">
        <magnitude><val>1081</val></magnitude>
       </node>
      </node>
      <node name="g__Lachnoclostridium">
       <magnitude><val>224957</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lachnoclostridium_phocaeense">
        <magnitude><val>9593</val></magnitude>
       </node>
       <node name="s__Lachnoclostridium_phytofermentans">
        <magnitude><val>1686</val></magnitude>
       </node>
       <node name="s__[Clostridium]_hylemonae">
        <magnitude><val>23228</val></magnitude>
       </node>
       <node name="s__[Clostridium]_scindens">
        <magnitude><val>190450</val></magnitude>
       </node>
      </node>
      <node name="g__Lachnospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>4565</val></magnitude>
       <node name="s__Lachnospira_eligens">
        <magnitude><val>4565</val></magnitude>
       </node>
      </node>
      <node name="g__Anaeromicropila">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1282</val></magnitude>
       <node name="s__Anaeromicropila_herbilytica">
        <magnitude><val>1282</val></magnitude>
       </node>
      </node>
      <node name="g__Butyrivibrio">
       <magnitude><val>29104</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Butyrivibrio_hungatei">
        <magnitude><val>3560</val></magnitude>
       </node>
       <node name="s__Butyrivibrio_proteoclasticus">
        <magnitude><val>1318</val></magnitude>
       </node>
       <node name="s__Butyrivibrio_crossotus">
        <magnitude><val>21551</val></magnitude>
       </node>
       <node name="s__Butyrivibrio_fibrisolvens">
        <magnitude><val>2675</val></magnitude>
       </node>
      </node>
      <node name="g__Roseburia">
       <magnitude><val>134305</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Roseburia_rectibacter">
        <magnitude><val>11241</val></magnitude>
       </node>
       <node name="s__Roseburia_hominis">
        <magnitude><val>32830</val></magnitude>
       </node>
       <node name="s__Roseburia_intestinalis">
        <magnitude><val>90234</val></magnitude>
       </node>
      </node>
      <node name="g__Stomatobaculum">
       <magnitude><val>925</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Stomatobaculum_sp._F0698">
        <magnitude><val>925</val></magnitude>
       </node>
      </node>
      <node name="g__Dorea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>333140</val></magnitude>
       <node name="s__Dorea_longicatena">
        <magnitude><val>116255</val></magnitude>
       </node>
       <node name="s__Dorea_formicigenerans">
        <magnitude><val>216885</val></magnitude>
       </node>
      </node>
      <node name="g__Simiaoa">
       <magnitude><val>25273</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Simiaoa_sunii">
        <magnitude><val>25273</val></magnitude>
       </node>
      </node>
      <node name="g__Claveliimonas">
       <magnitude><val>13257</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Claveliimonas_bilis">
        <magnitude><val>13257</val></magnitude>
       </node>
      </node>
      <node name="g__Sellimonas">
       <magnitude><val>13816</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sellimonas_intestinalis">
        <magnitude><val>13816</val></magnitude>
       </node>
      </node>
      <node name="g__Enterocloster">
       <magnitude><val>215728</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Enterocloster_bolteae">
        <magnitude><val>151155</val></magnitude>
       </node>
       <node name="s__Enterocloster_asparagiformis">
        <magnitude><val>16726</val></magnitude>
       </node>
       <node name="s__Enterocloster_clostridioformis">
        <magnitude><val>47847</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerobutyricum">
       <magnitude><val>531176</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaerobutyricum_hallii">
        <magnitude><val>531176</val></magnitude>
       </node>
      </node>
      <node name="g__Tyzzerella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>273</val></magnitude>
       <node name="s__[Clostridium]_colinum">
        <magnitude><val>273</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Epulonipiscium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>147</val></magnitude>
       <node name="s__Epulopiscium_sp._'N.t._morphotype_B'">
        <magnitude><val>147</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerocolumna">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10128</val></magnitude>
       <node name="s__Anaerocolumna_cellulosilytica">
        <magnitude><val>1766</val></magnitude>
       </node>
       <node name="s__Anaerocolumna_sedimenticola">
        <magnitude><val>1169</val></magnitude>
       </node>
       <node name="s__Anaerocolumna_chitinilytica">
        <magnitude><val>2226</val></magnitude>
       </node>
       <node name="s__Anaerocolumna_sp._AGMB13025">
        <magnitude><val>1588</val></magnitude>
       </node>
       <node name="s__Anaerocolumna_sp._AGMB13020">
        <magnitude><val>1651</val></magnitude>
       </node>
       <node name="s__Anaerocolumna_sp._MB42-C2">
        <magnitude><val>1728</val></magnitude>
       </node>
      </node>
      <node name="g__Wujia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>5188</val></magnitude>
       <node name="s__Wujia_chipingensis">
        <magnitude><val>5188</val></magnitude>
       </node>
      </node>
      <node name="g__Chakrabartyella">
       <magnitude><val>509</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Chakrabartyella_piscis">
        <magnitude><val>509</val></magnitude>
       </node>
      </node>
      <node name="g__Blautia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>4748363</val></magnitude>
       <node name="s__Blautia_pseudococcoides">
        <magnitude><val>10383</val></magnitude>
       </node>
       <node name="s__Blautia_wexlerae">
        <magnitude><val>3842305</val></magnitude>
       </node>
       <node name="s__Blautia_massiliensis_(ex_Durand_et_al._2017)">
        <magnitude><val>155986</val></magnitude>
       </node>
       <node name="s__Blautia_producta">
        <magnitude><val>23242</val></magnitude>
       </node>
       <node name="s__Blautia_parvula">
        <magnitude><val>76851</val></magnitude>
       </node>
       <node name="s__Blautia_hansenii">
        <magnitude><val>65759</val></magnitude>
       </node>
       <node name="s__Blautia_argi">
        <magnitude><val>100182</val></magnitude>
       </node>
       <node name="s__Blautia_sp._SC05B48">
        <magnitude><val>45783</val></magnitude>
       </node>
       <node name="s__Blautia_liquoris">
        <magnitude><val>2772</val></magnitude>
       </node>
       <node name="s__Blautia_obeum">
        <magnitude><val>145260</val></magnitude>
       </node>
       <node name="s__Blautia_luti">
        <magnitude><val>279840</val></magnitude>
       </node>
      </node>
      <node name="g__Wansuia">
       <magnitude><val>26701</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Wansuia_hejianensis">
        <magnitude><val>26701</val></magnitude>
       </node>
      </node>
      <node name="g__Qiania">
       <magnitude><val>9456</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Qiania_dongpingensis">
        <magnitude><val>9456</val></magnitude>
       </node>
      </node>
      <node name="g__Mediterraneibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1882568</val></magnitude>
       <node name="s__[Ruminococcus]_lactaris">
        <magnitude><val>29985</val></magnitude>
       </node>
       <node name="s__[Ruminococcus]_gnavus">
        <magnitude><val>1343459</val></magnitude>
       </node>
       <node name="s__[Ruminococcus]_torques">
        <magnitude><val>509124</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerostipes">
       <magnitude><val>983574</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaerostipes_hadrus">
        <magnitude><val>977441</val></magnitude>
       </node>
       <node name="s__Anaerostipes_rhamnosivorans">
        <magnitude><val>2133</val></magnitude>
       </node>
       <node name="s__Anaerostipes_caccae">
        <magnitude><val>4000</val></magnitude>
       </node>
      </node>
      <node name="g__Kineothrix">
       <magnitude><val>2003</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kineothrix_sp._MB12-C1">
        <magnitude><val>2003</val></magnitude>
       </node>
      </node>
      <node name="g__Herbinix">
       <magnitude><val>868</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Herbinix_luporum">
        <magnitude><val>868</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Clostridiales_Family_XVI._Incertae_Sedis">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>227</val></magnitude>
      <node name="g__Carboxydocella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>227</val></magnitude>
       <node name="s__Carboxydocella_thermautotrophica">
        <magnitude><val>227</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Proteinivoraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>34</val></magnitude>
      <node name="g__Alkalicella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>34</val></magnitude>
       <node name="s__Alkalicella_caledoniensis">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfotomaculaceae">
      <magnitude><val>32</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfotomaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>32</val></magnitude>
       <node name="s__Desulfotomaculum_nigrificans">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Maliibacteriaceae">
      <magnitude><val>476</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Maliibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>476</val></magnitude>
       <node name="s__Maliibacterium_massiliense">
        <magnitude><val>476</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Heliobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>298</val></magnitude>
      <node name="g__Heliorestis">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Heliorestis_convoluta">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
      <node name="g__Heliomicrobium">
       <magnitude><val>267</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Heliomicrobium_modesticaldum">
        <magnitude><val>267</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Flintibacter">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>2150</val></magnitude>
      <node name="s__Flintibacter_sp._KGMB00164">
       <magnitude><val>2150</val></magnitude>
      </node>
     </node>
     <node name="f__Peptostreptococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>101630</val></magnitude>
      <node name="g__Clostridioides">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>89560</val></magnitude>
       <node name="s__Clostridioides_difficile">
        <magnitude><val>89560</val></magnitude>
       </node>
      </node>
      <node name="g__Peptacetobacter">
       <magnitude><val>1713</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Peptacetobacter_hiranonis">
        <magnitude><val>1713</val></magnitude>
       </node>
      </node>
      <node name="g__Acetoanaerobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Acetoanaerobium_sticklandii">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Romboutsia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>6641</val></magnitude>
       <node name="s__Romboutsia_sp._CE17">
        <magnitude><val>254</val></magnitude>
       </node>
       <node name="s__Romboutsia_sp._13368">
        <magnitude><val>1091</val></magnitude>
       </node>
       <node name="s__Romboutsia_ilealis">
        <magnitude><val>5161</val></magnitude>
       </node>
       <node name="s__Romboutsia_hominis">
        <magnitude><val>135</val></magnitude>
       </node>
      </node>
      <node name="g__Terrisporobacter">
       <magnitude><val>431</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Terrisporobacter_mayombei">
        <magnitude><val>174</val></magnitude>
       </node>
       <node name="s__Terrisporobacter_hibernicus">
        <magnitude><val>138</val></magnitude>
       </node>
       <node name="s__Terrisporobacter_petrolearius">
        <magnitude><val>119</val></magnitude>
       </node>
      </node>
      <node name="g__Peptoclostridium">
       <magnitude><val>379</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Peptoclostridium_acidaminophilum">
        <magnitude><val>379</val></magnitude>
       </node>
      </node>
      <node name="g__Paeniclostridium">
       <magnitude><val>174</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paeniclostridium_sordellii">
        <magnitude><val>174</val></magnitude>
       </node>
      </node>
      <node name="g__Filifactor">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2323</val></magnitude>
       <node name="s__Filifactor_alocis">
        <magnitude><val>2323</val></magnitude>
       </node>
      </node>
      <node name="g__Tepidibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>188</val></magnitude>
       <node name="s__Tepidibacter_hydrothermalis">
        <magnitude><val>107</val></magnitude>
       </node>
       <node name="s__Tepidibacter_sp._8C15b">
        <magnitude><val>81</val></magnitude>
       </node>
      </node>
      <node name="g__Peptostreptococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>198</val></magnitude>
       <node name="s__Peptostreptococcus_sp._CBA3647">
        <magnitude><val>198</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Eubacteriaceae">
      <magnitude><val>39115</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Alkalibacter">
       <magnitude><val>247</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Alkalibacter_rhizosphaerae">
        <magnitude><val>247</val></magnitude>
       </node>
      </node>
      <node name="g__Eubacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27362</val></magnitude>
       <node name="s__Eubacterium_ventriosum">
        <magnitude><val>17893</val></magnitude>
       </node>
       <node name="s__Eubacterium_callanderi">
        <magnitude><val>2658</val></magnitude>
       </node>
       <node name="s__Eubacterium_maltosivorans">
        <magnitude><val>2611</val></magnitude>
       </node>
       <node name="s__Eubacterium_sp._MSJ-33">
        <magnitude><val>2546</val></magnitude>
       </node>
       <node name="s__Eubacterium_limosum">
        <magnitude><val>1654</val></magnitude>
       </node>
      </node>
      <node name="g__Intestinibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11072</val></magnitude>
       <node name="s__Intestinibacillus_sp._NTUH-41-i26">
        <magnitude><val>11072</val></magnitude>
       </node>
      </node>
      <node name="g__Acetobacterium">
       <magnitude><val>434</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Acetobacterium_woodii">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Acetobacterium_wieringae">
        <magnitude><val>263</val></magnitude>
       </node>
       <node name="s__Acetobacterium_sp._KB-1">
        <magnitude><val>123</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aristaeellaceae">
      <magnitude><val>960</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aristaeella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>960</val></magnitude>
       <node name="s__Aristaeella_hokkaidonensis">
        <magnitude><val>329</val></magnitude>
       </node>
       <node name="s__Aristaeella_lactis">
        <magnitude><val>631</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Intestinimonas">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>4769</val></magnitude>
      <node name="s__Intestinimonas_butyriciproducens">
       <magnitude><val>4769</val></magnitude>
      </node>
     </node>
     <node name="f__Eubacteriales_Family_XIII._Incertae_Sedis">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>8173</val></magnitude>
      <node name="g__Emergencia">
       <magnitude><val>3750</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Emergencia_timonensis">
        <magnitude><val>3750</val></magnitude>
       </node>
      </node>
      <node name="g__Aminipila">
       <magnitude><val>1424</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aminipila_butyrica">
        <magnitude><val>535</val></magnitude>
       </node>
       <node name="s__Aminipila_luticellarii">
        <magnitude><val>274</val></magnitude>
       </node>
       <node name="s__Aminipila_terrae">
        <magnitude><val>615</val></magnitude>
       </node>
      </node>
      <node name="g__Mogibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2999</val></magnitude>
       <node name="s__Mogibacterium_diversum">
        <magnitude><val>2566</val></magnitude>
       </node>
       <node name="s__Mogibacterium_neglectum">
        <magnitude><val>145</val></magnitude>
       </node>
       <node name="s__Mogibacterium_pumilum">
        <magnitude><val>288</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Symbiobacteriaceae">
      <magnitude><val>59</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Symbiobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>59</val></magnitude>
       <node name="s__Symbiobacterium_thermophilum">
        <magnitude><val>59</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Vallitaleaceae">
      <magnitude><val>2300</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Petrocella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>963</val></magnitude>
       <node name="s__Petrocella_atlantisensis">
        <magnitude><val>963</val></magnitude>
       </node>
      </node>
      <node name="g__Vallitalea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1337</val></magnitude>
       <node name="s__Vallitalea_guaymasensis">
        <magnitude><val>676</val></magnitude>
       </node>
       <node name="s__Vallitalea_pronyensis">
        <magnitude><val>661</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Proteiniborus">
      <magnitude><val>277</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Proteiniborus_sp._MB09-C3">
       <magnitude><val>277</val></magnitude>
      </node>
     </node>
     <node name="f__Peptococcaceae">
      <magnitude><val>909</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Dehalobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>102</val></magnitude>
       <node name="s__Dehalobacterium_formicoaceticum">
        <magnitude><val>102</val></magnitude>
       </node>
      </node>
      <node name="g__Desulforamulus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>674</val></magnitude>
       <node name="s__Desulforamulus_ruminis">
        <magnitude><val>134</val></magnitude>
       </node>
       <node name="s__Desulforamulus_ferrireducens">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Desulforamulus_reducens">
        <magnitude><val>525</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Formimonas">
       <magnitude><val>57</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Formimonas_warabiya">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Thermanaerosceptrum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>43</val></magnitude>
       <node name="s__Thermanaerosceptrum_fracticalcis">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
      <node name="g__Acididesulfobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Acididesulfobacillus_acetoxydans">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Desulforudis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Candidatus_Desulforudis_audaxviator">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Caldicellulosiruptorales">
     <magnitude><val>2327</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Caldicellulosiruptoraceae">
      <magnitude><val>2327</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Caldicellulosiruptor">
       <magnitude><val>2327</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caldicellulosiruptor_hydrothermalis">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_owensensis">
        <magnitude><val>255</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_diazotrophicus">
        <magnitude><val>694</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_bescii">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_saccharolyticus">
        <magnitude><val>106</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_morganii">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_acetigenus">
        <magnitude><val>350</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_changbaiensis">
        <magnitude><val>139</val></magnitude>
       </node>
       <node name="s__Caldicellulosiruptor_naganoensis">
        <magnitude><val>606</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Tissierellia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>11804</val></magnitude>
    <node name="o__Tissierellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11459</val></magnitude>
     <node name="f__Gottschalkiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>31</val></magnitude>
      <node name="g__Gottschalkia">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gottschalkia_acidurici">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Acidilutibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>142</val></magnitude>
      <node name="g__Acidilutibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>142</val></magnitude>
       <node name="s__Acidilutibacter_cellobiosedens">
        <magnitude><val>142</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Tepidimicrobiaceae">
      <magnitude><val>95</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Schnuerera">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Schnuerera_ultunensis">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Keratinibaculum">
       <magnitude><val>79</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Keratinibaculum_paraultunense">
        <magnitude><val>79</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Peptoniphilaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>10392</val></magnitude>
      <node name="g__Anaerococcus">
       <magnitude><val>594</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaerococcus_mediterraneensis">
        <magnitude><val>84</val></magnitude>
       </node>
       <node name="s__Anaerococcus_obesiensis">
        <magnitude><val>301</val></magnitude>
       </node>
       <node name="s__Anaerococcus_prevotii">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__Anaerococcus_sp._Marseille-Q7828">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Anaerococcus_vaginalis">
        <magnitude><val>150</val></magnitude>
       </node>
      </node>
      <node name="g__Peptoniphilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1979</val></magnitude>
       <node name="s__Peptoniphilus_ivorii">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Peptoniphilus_equinus">
        <magnitude><val>1198</val></magnitude>
       </node>
       <node name="s__Peptoniphilus_harei">
        <magnitude><val>610</val></magnitude>
       </node>
       <node name="s__Peptoniphilus_sp._SAHP1">
        <magnitude><val>110</val></magnitude>
       </node>
      </node>
      <node name="g__Parvimonas">
       <magnitude><val>1029</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parvimonas_micra">
        <magnitude><val>1029</val></magnitude>
       </node>
      </node>
      <node name="g__Miniphocaeibacter">
       <magnitude><val>113</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Miniphocaeibacter_halophilus">
        <magnitude><val>113</val></magnitude>
       </node>
      </node>
      <node name="g__Helcococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Helcococcus_kunzii">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Murdochiella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>6237</val></magnitude>
       <node name="s__Murdochiella_vaginalis">
        <magnitude><val>6237</val></magnitude>
       </node>
      </node>
      <node name="g__Finegoldia">
       <magnitude><val>407</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Finegoldia_magna">
        <magnitude><val>407</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Tissierellaceae">
      <magnitude><val>418</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gudongella">
       <magnitude><val>193</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gudongella_oleilytica">
        <magnitude><val>193</val></magnitude>
       </node>
      </node>
      <node name="g__Tissierella">
       <magnitude><val>225</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tissierella_sp._MB52-C2">
        <magnitude><val>139</val></magnitude>
       </node>
       <node name="s__Tissierella_sp._Yu-01">
        <magnitude><val>86</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermohalobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>381</val></magnitude>
      <node name="g__Caloranaerobacter">
       <magnitude><val>381</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caloranaerobacter_azorensis">
        <magnitude><val>381</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="g__Ezakiella">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>93</val></magnitude>
     <node name="s__Ezakiella_massiliensis">
      <magnitude><val>10</val></magnitude>
     </node>
     <node name="s__Ezakiella_coagulans">
      <magnitude><val>83</val></magnitude>
     </node>
    </node>
    <node name="g__Sedimentibacter">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>252</val></magnitude>
     <node name="s__Sedimentibacter_sp._MB35-C1">
      <magnitude><val>161</val></magnitude>
     </node>
     <node name="s__Sedimentibacter_sp._zth1">
      <magnitude><val>91</val></magnitude>
     </node>
    </node>
   </node>
   <node name="g__Ndongobacter">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>93</val></magnitude>
    <node name="s__Ndongobacter_massiliensis">
     <magnitude><val>93</val></magnitude>
    </node>
   </node>
   <node name="c__Dethiobacteria">
    <magnitude><val>26</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Dethiobacterales">
     <magnitude><val>26</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Dethiobacteraceae">
      <magnitude><val>26</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Contubernalis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Candidatus_Contubernalis_alkalaceticus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Armatimonadota">
   <magnitude><val>29</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Chthonomonadetes">
    <magnitude><val>29</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Chthonomonadales">
     <magnitude><val>29</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Chthonomonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>29</val></magnitude>
      <node name="g__Chthonomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Chthonomonas_calidirosea">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Pseudomonadota">
   <magnitude><val>60342</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Acidithiobacillia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>128</val></magnitude>
    <node name="o__Acidithiobacillales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>128</val></magnitude>
     <node name="f__Acidithiobacillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>128</val></magnitude>
      <node name="g__Acidithiobacillus">
       <magnitude><val>128</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Acidithiobacillus_sp._AMEEHan">
        <magnitude><val>128</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Hydrogenophilia">
    <magnitude><val>125</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Hydrogenophilales">
     <magnitude><val>125</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hydrogenophilaceae">
      <magnitude><val>125</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Hydrogenophilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>125</val></magnitude>
       <node name="s__Hydrogenophilus_thermoluteolus">
        <magnitude><val>125</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Betaproteobacteria">
    <magnitude><val>7180</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Nitrosomonadales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>424</val></magnitude>
     <node name="f__Sulfuricellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>26</val></magnitude>
      <node name="g__Sulfurimicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Sulfurimicrobium_lacus">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Sulfuriferula">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sulfuriferula_plumbiphila">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Gallionellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>23</val></magnitude>
      <node name="g__Gallionella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Gallionella_capsiferriformans">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methylophilaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>55</val></magnitude>
      <node name="g__Methylotenera">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methylotenera_mobilis">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Methylopumilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Candidatus_Methylopumilus_universalis">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sterolibacteriaceae">
      <magnitude><val>306</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Rugosibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>110</val></magnitude>
       <node name="s__Rugosibacter_aromaticivorans">
        <magnitude><val>110</val></magnitude>
       </node>
      </node>
      <node name="g__Sulfuritalea">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sulfuritalea_hydrogenivorans">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Denitratisoma">
       <magnitude><val>182</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Denitratisoma_oestradiolicum">
        <magnitude><val>157</val></magnitude>
       </node>
       <node name="s__Denitratisoma_sp._DHT3">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nitrosomonadaceae">
      <magnitude><val>14</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nitrosomonas">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nitrosomonas_eutropha">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Neisseriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1263</val></magnitude>
     <node name="f__Chitinibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>258</val></magnitude>
      <node name="g__Iodobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>125</val></magnitude>
       <node name="s__Iodobacter_fluviatilis">
        <magnitude><val>125</val></magnitude>
       </node>
      </node>
      <node name="g__Chitinibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>80</val></magnitude>
       <node name="s__Chitinibacter_bivalviorum">
        <magnitude><val>80</val></magnitude>
       </node>
      </node>
      <node name="g__Silvimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Silvimonas_soli">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Chitinimonas">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Chitinimonas_arctica">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aquaspirillaceae">
      <magnitude><val>61</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aquaspirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>61</val></magnitude>
       <node name="s__Aquaspirillum_sp._LM1">
        <magnitude><val>61</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Neisseriaceae">
      <magnitude><val>730</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Snodgrassella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__Snodgrassella_alvi">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Snodgrassella_communis">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Uruburuella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>45</val></magnitude>
       <node name="s__Uruburuella_testudinis">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Neisseria">
       <magnitude><val>638</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Neisseria_sp._DTU_2021_1001991_1_SI_NGA_ILE_055">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Neisseria_elongata">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Neisseria_animaloris">
        <magnitude><val>546</val></magnitude>
       </node>
       <node name="s__Neisseria_wadsworthii">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Wielerella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Wielerella_bovis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Chromobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>214</val></magnitude>
      <node name="g__Aquitalea">
       <magnitude><val>146</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aquitalea_magnusonii">
        <magnitude><val>146</val></magnitude>
       </node>
      </node>
      <node name="g__Chromobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>68</val></magnitude>
       <node name="s__Chromobacterium_sp._Beijing">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Chromobacterium_rhizoryzae">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="g__Candidatus_Kinetoplastibacterium">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>304</val></magnitude>
     <node name="s__Candidatus_Kinetoplastibacterium_sorsogonicusi">
      <magnitude><val>288</val></magnitude>
     </node>
     <node name="s__Candidatus_Kinetoplastibacterium_oncopeltii">
      <magnitude><val>16</val></magnitude>
     </node>
    </node>
    <node name="o__Burkholderiales">
     <magnitude><val>4250</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Eleftheria">
      <magnitude><val>14</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Eleftheria_terrae">
       <magnitude><val>14</val></magnitude>
      </node>
     </node>
     <node name="f__Comamonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>957</val></magnitude>
      <node name="g__Comamonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>87</val></magnitude>
       <node name="s__Comamonas_thiooxydans">
        <magnitude><val>70</val></magnitude>
       </node>
       <node name="s__Comamonas_terrigena">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Variovorax">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>461</val></magnitude>
       <node name="s__Variovorax_paradoxus">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Variovorax_sp._RKNM96">
        <magnitude><val>431</val></magnitude>
       </node>
      </node>
      <node name="g__Melaminivora">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>43</val></magnitude>
       <node name="s__Melaminivora_suipulveris">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
      <node name="g__Ottowia">
       <magnitude><val>118</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Ottowia_sp._SB7-C50">
        <magnitude><val>118</val></magnitude>
       </node>
      </node>
      <node name="g__Acidovorax">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>71</val></magnitude>
       <node name="s__Acidovorax_sp._RAC01">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Acidovorax_carolinensis">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Acidovorax_sp._NCPPB_3576">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Diaphorobacter">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Diaphorobacter_aerolatus">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Delftia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>113</val></magnitude>
       <node name="s__Delftia_lacustris">
        <magnitude><val>113</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodoferax">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rhodoferax_sp._AJA081-3">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__uncultured_Rhodoferax_sp.">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sutterellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1198</val></magnitude>
      <node name="g__Turicimonas">
       <magnitude><val>1026</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Turicimonas_muris">
        <magnitude><val>1026</val></magnitude>
       </node>
      </node>
      <node name="g__Sutterella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>92</val></magnitude>
       <node name="s__Sutterella_megalosphaeroides">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Sutterella_wadsworthensis">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Sutterella_faecalis">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Duodenibacillus">
       <magnitude><val>80</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Duodenibacillus_massiliensis">
        <magnitude><val>80</val></magnitude>
       </node>
      </node>
     </node>
     <node name="g__Xylophilus">
      <magnitude><val>20</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Xylophilus_rhododendri">
       <magnitude><val>20</val></magnitude>
      </node>
     </node>
     <node name="f__Burkholderiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1000</val></magnitude>
      <node name="g__Candidatus_Vallotia">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Vallotia_lariciata">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Burkholderia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>193</val></magnitude>
       <node name="s__Burkholderia_cepacia">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Burkholderia_multivorans">
        <magnitude><val>149</val></magnitude>
       </node>
      </node>
      <node name="g__Pandoraea">
       <magnitude><val>95</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pandoraea_pnomenusa">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Pandoraea_apista">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Pandoraea_vervacti">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Polynucleobacter">
       <magnitude><val>162</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Polynucleobacter_sp._AP-Kolm-20A-A1">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Polynucleobacter_necessarius">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Polynucleobacter_difficilis">
        <magnitude><val>53</val></magnitude>
       </node>
      </node>
      <node name="g__Paraburkholderia">
       <magnitude><val>186</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paraburkholderia_acidisoli">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Paraburkholderia_caribensis">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Paraburkholderia_fungorum">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Paraburkholderia_phenoliruptrix">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Cupriavidus">
       <magnitude><val>294</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cupriavidus_pauculus">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Cupriavidus_pinatubonensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Cupriavidus_sp._BIC8F">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Cupriavidus_taiwanensis">
        <magnitude><val>149</val></magnitude>
       </node>
       <node name="s__Cupriavidus_neocaledonicus">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Cupriavidus_nantongensis">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
      <node name="g__Limnobacter">
       <magnitude><val>50</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Limnobacter_sp._SAORIC-580">
        <magnitude><val>50</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sphaerotilaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>43</val></magnitude>
      <node name="g__Roseateles">
       <magnitude><val>43</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Roseateles_sp._SL47">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Roseateles_amylovorans">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Alcaligenaceae">
      <magnitude><val>649</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Bordetella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>143</val></magnitude>
       <node name="s__Bordetella_holmesii">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Bordetella_avium">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Bordetella_flabilis">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Bordetella_sp._N">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Bordetella_trematum">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Pusillimonas">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pusillimonas_sp._DMV24BSW_D">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Orrella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Orrella_dioscoreae">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Achromobacter">
       <magnitude><val>269</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Achromobacter_spanius">
        <magnitude><val>57</val></magnitude>
       </node>
       <node name="s__Achromobacter_insolitus">
        <magnitude><val>93</val></magnitude>
       </node>
       <node name="s__Achromobacter_deleyi">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Achromobacter_sp._B7">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Achromobacter_xylosoxidans">
        <magnitude><val>75</val></magnitude>
       </node>
      </node>
      <node name="g__Alcaligenes">
       <magnitude><val>158</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Alcaligenes_faecalis">
        <magnitude><val>158</val></magnitude>
       </node>
      </node>
      <node name="g__Pigmentiphaga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Pigmentiphaga_aceris">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Advenella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Advenella_kashmirensis">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Pelistega">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pelistega_ratti">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Oxalobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>369</val></magnitude>
      <node name="g__Collimonas">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Collimonas_arenae">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Collimonas_fungivorans">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Undibacterium">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Undibacterium_parvum">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Janthinobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>82</val></magnitude>
       <node name="s__Janthinobacterium_sp._17J80-10">
        <magnitude><val>47</val></magnitude>
       </node>
       <node name="s__Janthinobacterium_sp._J1-1">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
      <node name="g__Herbaspirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>46</val></magnitude>
       <node name="s__Herbaspirillum_hiltneri">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Herbaspirillum_rubrisubalbicans">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Herminiimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>56</val></magnitude>
       <node name="s__Herminiimonas_arsenitoxidans">
        <magnitude><val>56</val></magnitude>
       </node>
      </node>
      <node name="g__Massilia">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Massilia_violaceinigra">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
      <node name="g__Oxalobacter">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Oxalobacter_formigenes">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Oxalobacter_aliiformigenes">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Rugamonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>76</val></magnitude>
       <node name="s__Rugamonas_sp._DEMB1">
        <magnitude><val>76</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Rhodocyclales">
     <magnitude><val>939</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Azonexaceae">
      <magnitude><val>113</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Ferribacterium">
       <magnitude><val>113</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Ferribacterium_limneticum">
        <magnitude><val>113</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Zoogloeaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>781</val></magnitude>
      <node name="g__Parazoarcus">
       <magnitude><val>702</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parazoarcus_communis">
        <magnitude><val>702</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudothauera">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudothauera_hydrothermalis">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Thauera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Thauera_sp._GDN1">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
      <node name="g__Azoarcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__Azoarcus_sp._DN11">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Azoarcus_sp._KH32C">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Rhodocyclaceae">
      <magnitude><val>45</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aromatoleum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25</val></magnitude>
       <node name="s__Aromatoleum_bremense">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Azospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Azospira_inquinata">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Zetaproteobacteria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>355</val></magnitude>
    <node name="o__Mariprofundales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>355</val></magnitude>
     <node name="f__Mariprofundaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>355</val></magnitude>
      <node name="g__Mariprofundus">
       <magnitude><val>355</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mariprofundus_ferrinatatus">
        <magnitude><val>355</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Alphaproteobacteria">
    <magnitude><val>11956</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Hyphomicrobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>4532</val></magnitude>
     <node name="f__Devosiaceae">
      <magnitude><val>304</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Maritalea">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Maritalea_myrionectae">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Devosia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>256</val></magnitude>
       <node name="s__Devosia_sp._RR2S18">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Devosia_beringensis">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Devosia_sp._FJ2-5-3">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Devosia_neptuniae">
        <magnitude><val>62</val></magnitude>
       </node>
       <node name="s__Devosia_sp._SL43">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Pelagibacterium">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pelagibacterium_halotolerans">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Mariluticola">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Mariluticola_halotolerans">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bartonellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>366</val></magnitude>
      <node name="g__Bartonella">
       <magnitude><val>366</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Bartonella_ancashensis">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Bartonella_sp._TP">
        <magnitude><val>327</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nitrobacteraceae">
      <magnitude><val>421</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Bradyrhizobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>347</val></magnitude>
       <node name="s__Bradyrhizobium_erythrophlei">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Bradyrhizobium_sp._BWA-3-5">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Bradyrhizobium_betae">
        <magnitude><val>120</val></magnitude>
       </node>
       <node name="s__Bradyrhizobium_sp._NP1">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Bradyrhizobium_diazoefficiens">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Bradyrhizobium_australafricanum">
        <magnitude><val>106</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodopseudomonas">
       <magnitude><val>74</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rhodopseudomonas_palustris">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Stappiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>203</val></magnitude>
      <node name="g__Pannonibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>47</val></magnitude>
       <node name="s__Pannonibacter_phragmitetus">
        <magnitude><val>47</val></magnitude>
       </node>
      </node>
      <node name="g__Roseibium">
       <magnitude><val>39</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Roseibium_sp._Sym1">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
      <node name="g__Stappia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>117</val></magnitude>
       <node name="s__Stappia_sp._ES.058">
        <magnitude><val>117</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Breoghaniaceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Breoghania">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Breoghania_sp._L-A4">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Cohaesibacteraceae">
      <magnitude><val>242</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cohaesibacter">
       <magnitude><val>242</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cohaesibacter_sp._ES.047">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__uncultured_Cohaesibacter_sp.">
        <magnitude><val>198</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Rhizobiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1356</val></magnitude>
      <node name="g__Sinorhizobium">
       <magnitude><val>59</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sinorhizobium_meliloti">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Sinorhizobium_sp._BG8">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Agrobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>231</val></magnitude>
       <node name="s__Agrobacterium_fabacearum">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Agrobacterium_pusense">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Agrobacterium_vaccinii">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Agrobacterium_fabrum">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Agrobacterium_tumefaciens">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Agrobacterium_vitis">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Rhizobium">
       <magnitude><val>884</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rhizobium_sp._WL3">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Rhizobium_leguminosarum">
        <magnitude><val>168</val></magnitude>
       </node>
       <node name="s__Rhizobium_lusitanum">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Rhizobium_rhizogenes">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Rhizobium_binae">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Rhizobium_tropici">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Rhizobium_sp._BT-226">
        <magnitude><val>549</val></magnitude>
       </node>
      </node>
      <node name="g__Gellertiella">
       <magnitude><val>30</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Gellertiella_sp.">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Shinella">
       <magnitude><val>152</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Shinella_zoogloeoides">
        <magnitude><val>152</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Xanthobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>33</val></magnitude>
      <node name="g__Pseudolabrys">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudolabrys_sp._FHR47">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Azorhizobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Azorhizobium_caulinodans">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Chelatococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>16</val></magnitude>
      <node name="g__Chelatococcus">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Chelatococcus_daeguensis">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Brucellaceae">
      <magnitude><val>332</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Brucella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>107</val></magnitude>
       <node name="s__Brucella_sp._NM4">
        <magnitude><val>107</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudochrobactrum">
       <magnitude><val>225</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudochrobactrum_sp._XF203">
        <magnitude><val>225</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Phyllobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>517</val></magnitude>
      <node name="g__Lentilitoribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>380</val></magnitude>
       <node name="s__Lentilitoribacter_sp._Alg239-R112">
        <magnitude><val>380</val></magnitude>
       </node>
      </node>
      <node name="g__Mesorhizobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>137</val></magnitude>
       <node name="s__Mesorhizobium_sp._8">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Mesorhizobium_sp._B2-1-1">
        <magnitude><val>117</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Boseaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>76</val></magnitude>
      <node name="g__Bosea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>76</val></magnitude>
       <node name="s__Bosea_sp._RAC05">
        <magnitude><val>76</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methylocystaceae">
      <magnitude><val>276</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methylosinus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>218</val></magnitude>
       <node name="s__Methylosinus_sp._C49">
        <magnitude><val>218</val></magnitude>
       </node>
      </node>
      <node name="g__Methylocystis">
       <magnitude><val>58</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methylocystis_bryophila">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Methylocystis_heyeri">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Kaistiaceae">
      <magnitude><val>28</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Kaistia">
       <magnitude><val>28</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kaistia_sp._32K">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methylobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>65</val></magnitude>
      <node name="g__Microvirga">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Microvirga_sp._17_mud_1-3">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Methylobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>34</val></magnitude>
       <node name="s__Methylobacterium_indicum">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Methylorubrum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Methylorubrum_sp._B1-46">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Lichenihabitantaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>53</val></magnitude>
      <node name="g__Lichenihabitans">
       <magnitude><val>53</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lichenihabitans_psoromatis">
        <magnitude><val>53</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Hyphomicrobiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>49</val></magnitude>
      <node name="g__Rhodomicrobium">
       <magnitude><val>36</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rhodomicrobium_lacus">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Rhodomicrobium_vannielii">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Hyphomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Hyphomicrobium_sp._DMF-1">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Beijerinckiaceae">
      <magnitude><val>59</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Beijerinckia">
       <magnitude><val>46</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Beijerinckia_indica">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Methylovirgula">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Methylovirgula_sp._HY1">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aurantimonadaceae">
      <magnitude><val>123</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aureimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>54</val></magnitude>
       <node name="s__Aureimonas_sp._SA4125">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Aureimonas_sp._AU20">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
      <node name="g__Martelella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>69</val></magnitude>
       <node name="s__Martelella_sp._AD-3">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__uncultured_Martelella_sp.">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Holosporales">
     <magnitude><val>103</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Holosporaceae">
      <magnitude><val>103</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Nesciobacter">
       <magnitude><val>56</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Nesciobacter_abundans">
        <magnitude><val>56</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Hydrogenosomobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>47</val></magnitude>
       <node name="s__Candidatus_Hydrogenosomobacter_endosymbioticus">
        <magnitude><val>47</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Hyphomonadales">
     <magnitude><val>67</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hyphomonadaceae">
      <magnitude><val>67</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Hyphomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Hyphomonas_sp._Mor2">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Hirschia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>49</val></magnitude>
       <node name="s__Hirschia_baltica">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Kordiimonadales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>265</val></magnitude>
     <node name="f__Kordiimonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>32</val></magnitude>
      <node name="g__Kordiimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>32</val></magnitude>
       <node name="s__Kordiimonas_sp._SCSIO_12610">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Temperatibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>233</val></magnitude>
      <node name="g__Temperatibacter">
       <magnitude><val>233</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Temperatibacter_marinus">
        <magnitude><val>233</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Rhodobacterales">
     <magnitude><val>1108</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Paracoccaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>673</val></magnitude>
      <node name="g__Pelagovum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Pelagovum_pacificum">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Cognatishimia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Cognatishimia_activa">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudopuniceibacterium">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudopuniceibacterium_antarcticum">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Abyssibius">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>72</val></magnitude>
       <node name="s__Abyssibius_alkaniclasticus">
        <magnitude><val>72</val></magnitude>
       </node>
      </node>
      <node name="g__Parasedimentitalea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>32</val></magnitude>
       <node name="s__Parasedimentitalea_psychrophila">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Falsirhodobacter">
       <magnitude><val>23</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Falsirhodobacter_algicola">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Roseinatronobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>99</val></magnitude>
       <node name="s__Roseinatronobacter_sp._S2">
        <magnitude><val>99</val></magnitude>
       </node>
      </node>
      <node name="g__Paracoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>266</val></magnitude>
       <node name="s__Paracoccus_sediminicola">
        <magnitude><val>127</val></magnitude>
       </node>
       <node name="s__Paracoccus_sanguinis">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Paracoccus_sp._TOH">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Paracoccus_kondratievae">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Fuscovulum">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Fuscovulum_sp._YMD61">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodobacter">
       <magnitude><val>70</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rhodobacter_capsulatus">
        <magnitude><val>70</val></magnitude>
       </node>
      </node>
      <node name="g__Tritonibacter">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tritonibacter_mobilis">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Aliiroseovarius">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Aliiroseovarius_sp._M344">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Qingshengfaniella">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Qingshengfaniella_alkalisoli">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Roseobacteraceae">
      <magnitude><val>435</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Roseivivax">
       <magnitude><val>38</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Roseivivax_sp._THAF30">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Phaeobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Phaeobacter_inhibens">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Alloyangia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Alloyangia_pacifica">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Ruegeria">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Ruegeria_conchae">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Sulfitobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>149</val></magnitude>
       <node name="s__Sulfitobacter_alexandrii">
        <magnitude><val>104</val></magnitude>
       </node>
       <node name="s__Sulfitobacter_sp._BSw21498">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanicola">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Oceanicola_sp._D3">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Roseobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Roseobacter_ponti">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Roseobacter_litoralis">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Salipiger">
       <magnitude><val>29</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Salipiger_abyssi">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
      <node name="g__Leisingera">
       <magnitude><val>49</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leisingera_caerulea">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Leisingera_aquaemixtae">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Celeribacter">
       <magnitude><val>51</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Celeribacter_sp.">
        <magnitude><val>51</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Parvularculales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>235</val></magnitude>
     <node name="f__Parvularculaceae">
      <magnitude><val>235</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aquisalinus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>39</val></magnitude>
       <node name="s__Aquisalinus_flavus">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
      <node name="g__Parvularcula">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Parvularcula_sp._LCG005">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Hyphococcus">
       <magnitude><val>173</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Hyphococcus_flavus">
        <magnitude><val>173</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Rhodospirillales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>2696</val></magnitude>
     <node name="f__Thalassobaculaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>13</val></magnitude>
      <node name="g__Nisaea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Nisaea_acidiphila">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thalassospiraceae">
      <magnitude><val>455</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Magnetospira">
       <magnitude><val>24</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Magnetospira_sp._QH-2">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Thalassospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>411</val></magnitude>
       <node name="s__Thalassospira_marina">
        <magnitude><val>411</val></magnitude>
       </node>
      </node>
      <node name="g__Varunaivibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Varunaivibrio_sulfuroxidans">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Rhodospirillaceae">
      <magnitude><val>44</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Magnetospirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>44</val></magnitude>
       <node name="s__Magnetospirillum_sp._ME-1">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Magnetospirillum_gryphiswaldense">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Azospirillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>201</val></magnitude>
      <node name="g__Niveispirillum">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Niveispirillum_cyanobacteriorum">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Azospirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>153</val></magnitude>
       <node name="s__Azospirillum_brasilense">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Azospirillum_sp._TSH58">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Azospirillum_thermophilum">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
      <node name="g__Skermanella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Skermanella_mucosa">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Terasakiellaceae">
      <magnitude><val>196</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Terasakiella">
       <magnitude><val>196</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Terasakiella_sp._SH-1">
        <magnitude><val>196</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Kiloniellaceae">
      <magnitude><val>22</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aestuariispira">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aestuariispira_ectoiniformans">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Acetobacteraceae">
      <magnitude><val>1765</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Kozakia">
       <magnitude><val>38</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kozakia_baliensis">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Novacetimonas">
       <magnitude><val>124</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Novacetimonas_hansenii">
        <magnitude><val>124</val></magnitude>
       </node>
      </node>
      <node name="g__Roseococcus">
       <magnitude><val>52</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Roseococcus_microcysteis">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
      <node name="g__Acidocella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Acidocella_sp._MX-AZ03">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Aristophania">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>419</val></magnitude>
       <node name="s__Aristophania_vespae">
        <magnitude><val>419</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodovastum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Rhodovastum_atsumiense">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Granulibacter">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Granulibacter_bethesdensis">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Komagataeibacter">
       <magnitude><val>1020</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Komagataeibacter_rhaeticus">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Komagataeibacter_oboediens">
        <magnitude><val>970</val></magnitude>
       </node>
      </node>
      <node name="g__Gluconacetobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Gluconacetobacter_diazotrophicus">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Gluconobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>30</val></magnitude>
       <node name="s__Gluconobacter_oxydans">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Maricaulales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>12</val></magnitude>
     <node name="f__Maricaulaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>12</val></magnitude>
      <node name="g__Maricaulis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Maricaulis_maris">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Rickettsiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>147</val></magnitude>
     <node name="f__Rickettsiaceae">
      <magnitude><val>52</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Rickettsia">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rickettsia_endosymbiont_of_Ceutorhynchus_assimilis">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Orientia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>30</val></magnitude>
       <node name="s__Orientia_tsutsugamushi">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Anaplasmataceae">
      <magnitude><val>95</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Anaplasma">
       <magnitude><val>69</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Anaplasma_marginale">
        <magnitude><val>69</val></magnitude>
       </node>
      </node>
      <node name="g__Neorickettsia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Neorickettsia_helminthoeca">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Candidatus_Pelagibacterales">
     <magnitude><val>160</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Candidatus_Fonsibacter">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>10</val></magnitude>
      <node name="s__Candidatus_Fonsibacter_ubiquis">
       <magnitude><val>10</val></magnitude>
      </node>
     </node>
     <node name="f__Candidatus_Pelagibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>150</val></magnitude>
      <node name="g__Candidatus_Pelagibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>150</val></magnitude>
       <node name="s__Candidatus_Pelagibacter_sp._IMCC9063">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Candidatus_Pelagibacter_sp._RS40">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Candidatus_Pelagibacter_sp._RS39">
        <magnitude><val>79</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Caulobacterales">
     <magnitude><val>195</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Caulobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>195</val></magnitude>
      <node name="g__Brevundimonas">
       <magnitude><val>83</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Brevundimonas_sp.">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Brevundimonas_sp._AJA228-03">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Brevundimonas_vitisensis">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Caulobacter">
       <magnitude><val>26</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Caulobacter_sp._S6">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Asticcacaulis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>86</val></magnitude>
       <node name="s__Asticcacaulis_sp._SL142">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Asticcacaulis_excentricus">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Sphingomonadales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>2423</val></magnitude>
     <node name="f__Zymomonadaceae">
      <magnitude><val>10</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Zymomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Zymomonas_mobilis">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sphingomonadaceae">
      <magnitude><val>1606</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Allosphingosinicella">
       <magnitude><val>303</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Allosphingosinicella_indica">
        <magnitude><val>303</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingorhabdus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>39</val></magnitude>
       <node name="s__Sphingorhabdus_lacus">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Sphingorhabdus_lutea">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Parasphingopyxis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>102</val></magnitude>
       <node name="s__Parasphingopyxis_sp._CP4">
        <magnitude><val>102</val></magnitude>
       </node>
      </node>
      <node name="g__Rhizorhabdus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Rhizorhabdus_phycosphaerae">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingosinithalassobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Sphingosinithalassobacter_sp._CS137">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Hankyongella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>49</val></magnitude>
       <node name="s__Hankyongella_ginsenosidimutans">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
      <node name="g__Novosphingobium">
       <magnitude><val>69</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Novosphingobium_sp._P6W">
        <magnitude><val>53</val></magnitude>
       </node>
       <node name="s__Novosphingobium_humi">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Parasphingorhabdus">
       <magnitude><val>37</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parasphingorhabdus_halotolerans">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Parasphingorhabdus_litoris">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>130</val></magnitude>
       <node name="s__Sphingobium_sp._YG1">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Sphingobium_sp._KCTC_72723">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Sphingobium_sp._RAC03">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Sphingobium_sp._V4">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingomonas">
       <magnitude><val>240</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sphingomonas_hankookensis">
        <magnitude><val>102</val></magnitude>
       </node>
       <node name="s__Sphingomonas_sp.">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Sphingomonas_cannabina">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Sphingomonas_glaciei">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Sphingomonas_sp._AP4-R1">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingopyxis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>604</val></magnitude>
       <node name="s__Sphingopyxis_sp._113P3">
        <magnitude><val>563</val></magnitude>
       </node>
       <node name="s__Sphingopyxis_granuli">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Erythrobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>807</val></magnitude>
      <node name="g__Qipengyuania">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>22</val></magnitude>
       <node name="s__Qipengyuania_psychrotolerans">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Altererythrobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Altererythrobacter_sp._B11">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Altererythrobacter_sp._ZODW24">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Alteriqipengyuania">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Alteriqipengyuania_flavescens">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Croceibacterium">
       <magnitude><val>68</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Croceibacterium_atlanticum">
        <magnitude><val>68</val></magnitude>
       </node>
      </node>
      <node name="g__Erythrobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>674</val></magnitude>
       <node name="s__Erythrobacter_litoralis">
        <magnitude><val>639</val></magnitude>
       </node>
       <node name="s__Erythrobacter_sp.">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Emcibacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>13</val></magnitude>
     <node name="f__Emcibacteraceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Paremcibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Paremcibacter_congregatus">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Gammaproteobacteria">
    <magnitude><val>40598</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Acidiferrobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>45</val></magnitude>
     <node name="f__Acidiferrobacteraceae">
      <magnitude><val>45</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Sulfurifustis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>45</val></magnitude>
       <node name="s__Sulfurifustis_variabilis">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Pseudomonadales">
     <magnitude><val>3430</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Pseudomonadaceae">
      <magnitude><val>3218</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Stutzerimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>147</val></magnitude>
       <node name="s__Stutzerimonas_stutzeri">
        <magnitude><val>147</val></magnitude>
       </node>
      </node>
      <node name="g__Halopseudomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>498</val></magnitude>
       <node name="s__Halopseudomonas_sp._SMJS2">
        <magnitude><val>473</val></magnitude>
       </node>
       <node name="s__Pseudomonas_denitrificans_(nom._rej.)">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Entomomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>30</val></magnitude>
       <node name="s__Entomomonas_moraniae">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Entomomonas_asaccharolytica">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2543</val></magnitude>
       <node name="s__Pseudomonas_moraviensis">
        <magnitude><val>265</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._GR_6-02">
        <magnitude><val>159</val></magnitude>
       </node>
       <node name="s__Pseudomonas_frederiksbergensis">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._PSE14">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Pseudomonas_palleroniana">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Pseudomonas_putida">
        <magnitude><val>135</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._MTM4">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Pseudomonas_tohonis">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Pseudomonas_phytophila">
        <magnitude><val>72</val></magnitude>
       </node>
       <node name="s__Pseudomonas_entomophila">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._ADAK18">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._M30-35">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Pseudomonas_vancouverensis">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Pseudomonas_fulva">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Pseudomonas_saudiphocaensis">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._R76">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Pseudomonas_mendocina">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Pseudomonas_fluorescens">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Pseudomonas_asturiensis">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Pseudomonas_pohangensis">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Pseudomonas_luteola">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Pseudomonas_chlororaphis">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Pseudomonas_protegens">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Pseudomonas_poae">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._MM227">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._URMO17WK12:I11">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Pseudomonas_aeruginosa">
        <magnitude><val>541</val></magnitude>
       </node>
       <node name="s__Pseudomonas_psychrotolerans">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Pseudomonas_resinovorans">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Pseudomonas_orientalis">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Pseudomonas_toyotomiensis">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Pseudomonas_syringae">
        <magnitude><val>255</val></magnitude>
       </node>
       <node name="s__Pseudomonas_sp._FP1742">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Pseudomonas_lurida">
        <magnitude><val>459</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Marinobacteraceae">
      <magnitude><val>212</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Marinobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>212</val></magnitude>
       <node name="s__Marinobacter_sp._CA1">
        <magnitude><val>99</val></magnitude>
       </node>
       <node name="s__Marinobacter_shengliensis">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Marinobacter_nauticus">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Marinobacter_sp._LPB0319">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Cellvibrionales">
     <magnitude><val>938</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Microbulbiferaceae">
      <magnitude><val>232</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Microbulbifer">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>232</val></magnitude>
       <node name="s__Microbulbifer_elongatus">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Microbulbifer_aggregans">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Microbulbifer_sp._GL-2">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Microbulbifer_sp._YPW16">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Microbulbifer_agarilyticus">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Microbulbifer_thermotolerans">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Microbulbifer_sp._THAF38">
        <magnitude><val>70</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Halieaceae">
      <magnitude><val>49</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Halioglobus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>49</val></magnitude>
       <node name="s__Halioglobus_maricola">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Halioglobus_japonicus">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Cellvibrionaceae">
      <magnitude><val>657</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Teredinibacter">
       <magnitude><val>545</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Teredinibacter_turnerae">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Teredinibacter_sp._KSP-S5-2">
        <magnitude><val>509</val></magnitude>
       </node>
      </node>
      <node name="g__Marinimicrobium">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marinimicrobium_sp._C6131">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Cellvibrio">
       <magnitude><val>96</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cellvibrio_sp._KY-YJ-3">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Cellvibrio_sp._PSBB023">
        <magnitude><val>67</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="g__Gallaecimonas">
     <magnitude><val>152</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="s__Gallaecimonas_kandeliae">
      <magnitude><val>152</val></magnitude>
     </node>
    </node>
    <node name="o__Pasteurellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>852</val></magnitude>
     <node name="f__Pasteurellaceae">
      <magnitude><val>852</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gallibacterium">
       <magnitude><val>112</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gallibacterium_salpingitidis">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Gallibacterium_anatis">
        <magnitude><val>94</val></magnitude>
       </node>
      </node>
      <node name="g__Histophilus">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Histophilus_somni">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Mannheimia">
       <magnitude><val>294</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mannheimia_varigena">
        <magnitude><val>128</val></magnitude>
       </node>
       <node name="s__Mannheimia_granulomatis">
        <magnitude><val>166</val></magnitude>
       </node>
      </node>
      <node name="g__Pasteurella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Pasteurella_multocida">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Otariodibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>52</val></magnitude>
       <node name="s__Otariodibacter_oris">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
      <node name="g__Aggregatibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>40</val></magnitude>
       <node name="s__Aggregatibacter_aphrophilus">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Aggregatibacter_actinomycetemcomitans">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Avibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>98</val></magnitude>
       <node name="s__Avibacterium_volantium">
        <magnitude><val>98</val></magnitude>
       </node>
      </node>
      <node name="g__Rodentibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Rodentibacter_haemolyticus">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Haemophilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>174</val></magnitude>
       <node name="s__Haemophilus_pittmaniae">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Haemophilus_parainfluenzae">
        <magnitude><val>75</val></magnitude>
       </node>
       <node name="s__Haemophilus_parahaemolyticus">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Moraxellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1360</val></magnitude>
     <node name="f__Moraxellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1360</val></magnitude>
      <node name="g__Psychrobacter">
       <magnitude><val>97</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Psychrobacter_sp._WB2">
        <magnitude><val>97</val></magnitude>
       </node>
      </node>
      <node name="g__Moraxella">
       <magnitude><val>181</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Moraxella_osloensis">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Moraxella_sp._ZY171148">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Moraxella_sp._1_DOX410">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Moraxella_bovoculi">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Moraxella_nasibovis">
        <magnitude><val>102</val></magnitude>
       </node>
      </node>
      <node name="g__Acinetobacter">
       <magnitude><val>1082</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Acinetobacter_sp._KCTC_92772">
        <magnitude><val>106</val></magnitude>
       </node>
       <node name="s__Acinetobacter_sp._TTH0-4">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Acinetobacter_sp._PK01">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Acinetobacter_towneri">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Acinetobacter_sp._NCu2D-2">
        <magnitude><val>94</val></magnitude>
       </node>
       <node name="s__Acinetobacter_sp._ESL0695">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Acinetobacter_radioresistens">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Acinetobacter_pittii">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Acinetobacter_defluvii">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Acinetobacter_wanghuae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Acinetobacter_johnsonii">
        <magnitude><val>148</val></magnitude>
       </node>
       <node name="s__Acinetobacter_equi">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Acinetobacter_schindleri">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Acinetobacter_lactucae">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Acinetobacter_dispersus">
        <magnitude><val>81</val></magnitude>
       </node>
       <node name="s__Acinetobacter_baumannii">
        <magnitude><val>216</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Legionellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>546</val></magnitude>
     <node name="f__Legionellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>535</val></magnitude>
      <node name="g__Fluoribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>98</val></magnitude>
       <node name="s__Fluoribacter_dumoffii">
        <magnitude><val>98</val></magnitude>
       </node>
      </node>
      <node name="g__Legionella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>437</val></magnitude>
       <node name="s__Legionella_antarctica">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Legionella_geestiana">
        <magnitude><val>57</val></magnitude>
       </node>
       <node name="s__Legionella_pneumophila">
        <magnitude><val>153</val></magnitude>
       </node>
       <node name="s__Legionella_spiritensis">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Legionella_oakridgensis">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Legionella_israelensis">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Legionella_lansingensis">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Legionella_fallonii">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Coxiellaceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Coxiella-like_endosymbiont">
       <magnitude><val>11</val></magnitude>
      </node>
     </node>
    </node>
    <node name="o__Aeromonadales">
     <magnitude><val>1617</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Aeromonadaceae">
      <magnitude><val>1090</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aeromonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1077</val></magnitude>
       <node name="s__Aeromonas_media">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Aeromonas_salmonicida">
        <magnitude><val>165</val></magnitude>
       </node>
       <node name="s__Aeromonas_encheleia">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Aeromonas_hydrophila">
        <magnitude><val>807</val></magnitude>
       </node>
       <node name="s__Aeromonas_enteropelogenes">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Aeromonas_jandaei">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Aeromonas_veronii">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Oceanimonas_pelagia">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Succinivibrionaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>527</val></magnitude>
      <node name="g__Succinivibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>527</val></magnitude>
       <node name="s__Succinivibrio_dextrinosolvens">
        <magnitude><val>527</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Xanthomonadales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>579</val></magnitude>
     <node name="f__Xanthomonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>564</val></magnitude>
      <node name="g__Stenotrophomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>117</val></magnitude>
       <node name="s__Stenotrophomonas_maltophilia">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Stenotrophomonas_sp._364">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudoxanthomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>70</val></magnitude>
       <node name="s__Pseudoxanthomonas_sp._SE1">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Pseudoxanthomonas_sp._X-1">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
      <node name="g__Xanthomonas">
       <magnitude><val>322</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Xanthomonas_citri">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Xanthomonas_albilineans">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Xanthomonas_sp._CFBP_8445">
        <magnitude><val>92</val></magnitude>
       </node>
       <node name="s__Xanthomonas_sacchari">
        <magnitude><val>69</val></magnitude>
       </node>
       <node name="s__Xanthomonas_vasicola">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Xanthomonas_dyei">
        <magnitude><val>61</val></magnitude>
       </node>
      </node>
      <node name="g__Lysobacter">
       <magnitude><val>55</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lysobacter_solisilvae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Lysobacter_sp._H21R4">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Lysobacter_soli">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Rhodanobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>15</val></magnitude>
      <node name="g__Rhodanobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Rhodanobacter_thiooxydans">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Vibrionales">
     <magnitude><val>3909</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Vibrionaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>3909</val></magnitude>
      <node name="g__Salinivibrio">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Salinivibrio_kushneri">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Photobacterium">
       <magnitude><val>1112</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Photobacterium_sp._CCB-ST2H9">
        <magnitude><val>53</val></magnitude>
       </node>
       <node name="s__Photobacterium_atrarenae">
        <magnitude><val>231</val></magnitude>
       </node>
       <node name="s__Photobacterium_sp._GJ3">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Photobacterium_damselae">
        <magnitude><val>530</val></magnitude>
       </node>
       <node name="s__Photobacterium_sp._TLY01">
        <magnitude><val>197</val></magnitude>
       </node>
       <node name="s__Photobacterium_leiognathi">
        <magnitude><val>77</val></magnitude>
       </node>
      </node>
      <node name="g__Vibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2660</val></magnitude>
       <node name="s__uncultured_Vibrio_sp.">
        <magnitude><val>63</val></magnitude>
       </node>
       <node name="s__Vibrio_breoganii">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Vibrio_quintilis">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Vibrio_paracholerae">
        <magnitude><val>135</val></magnitude>
       </node>
       <node name="s__Vibrio_gazogenes">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Vibrio_plantisponsor">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Vibrio_anguillarum">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Vibrio_coralliilyticus">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__Vibrio_porteresiae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Vibrio_tritonius">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Vibrio_sp._SS-MA-C1-2">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Vibrio_owensii">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Vibrio_nigripulchritudo">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Vibrio_casei">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Vibrio_echinoideorum">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Vibrio_cyclitrophicus">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Vibrio_ruber">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Vibrio_parahaemolyticus">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Vibrio_zhugei">
        <magnitude><val>429</val></magnitude>
       </node>
       <node name="s__Vibrio_navarrensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Vibrio_sp._STUT-A16">
        <magnitude><val>409</val></magnitude>
       </node>
       <node name="s__Vibrio_sp._SCSIO_43137">
        <magnitude><val>80</val></magnitude>
       </node>
       <node name="s__Vibrio_vulnificus">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Vibrio_astriarenae">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Vibrio_gangliei">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Vibrio_ponticus">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Vibrio_cincinnatiensis">
        <magnitude><val>86</val></magnitude>
       </node>
       <node name="s__Vibrio_neptunius">
        <magnitude><val>179</val></magnitude>
       </node>
       <node name="s__Vibrio_azureus">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Vibrio_mimicus">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Vibrio_sp._YMD68">
        <magnitude><val>124</val></magnitude>
       </node>
       <node name="s__Vibrio_neonatus">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Vibrio_aquimaris">
        <magnitude><val>417</val></magnitude>
       </node>
      </node>
      <node name="g__Grimontia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Grimontia_hollisae">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Aliivibrio">
       <magnitude><val>97</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aliivibrio_fischeri">
        <magnitude><val>97</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Thiotrichales">
     <magnitude><val>364</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Thiotrichaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>159</val></magnitude>
      <node name="g__Beggiatoa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>143</val></magnitude>
       <node name="s__Beggiatoa_leptomitoformis">
        <magnitude><val>143</val></magnitude>
       </node>
      </node>
      <node name="g__Thiothrix">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thiothrix_lacustris">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Piscirickettsiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>205</val></magnitude>
      <node name="g__Thiomicrospira">
       <magnitude><val>70</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thiomicrospira_microaerophila">
        <magnitude><val>70</val></magnitude>
       </node>
      </node>
      <node name="g__Thiomicrorhabdus">
       <magnitude><val>59</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thiomicrorhabdus_aquaedulcis">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Thiomicrorhabdus_sp.">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Thiomicrorhabdus_immobilis">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Methylophaga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>76</val></magnitude>
       <node name="s__Methylophaga_pinxianii">
        <magnitude><val>76</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="g__Candidatus_Vesicomyosocius">
     <magnitude><val>139</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="s__Candidatus_Vesicomyosocius_okutanii">
      <magnitude><val>139</val></magnitude>
     </node>
    </node>
    <node name="o__Enterobacterales">
     <magnitude><val>23388</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Enterobacteriaceae">
      <magnitude><val>20559</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Blochmannia">
       <magnitude><val>477</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Blochmannia_vafer">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Blochmannia_endosymbiont_of_Colobopsis_nipponica">
        <magnitude><val>422</val></magnitude>
       </node>
      </node>
      <node name="s__Enterobacteriaceae_endosymbiont_of_Donacia_sparganii">
       <magnitude><val>15</val></magnitude>
      </node>
      <node name="s__Enterobacteriaceae_endosymbiont_of_Macroplea_mutica">
       <magnitude><val>12</val></magnitude>
      </node>
      <node name="g__Symbiopectobacterium">
       <magnitude><val>25</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Symbiopectobacterium_purcellii">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Ishikawaella">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Ishikawaella_capsulata">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Buttiauxella">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Buttiauxella_sp._R73">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Escherichia">
       <magnitude><val>13989</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Escherichia_albertii">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Escherichia_coli">
        <magnitude><val>13476</val></magnitude>
       </node>
       <node name="s__Escherichia_fergusonii">
        <magnitude><val>502</val></magnitude>
       </node>
      </node>
      <node name="g__Citrobacter">
       <magnitude><val>542</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Citrobacter_sp._RHB25-C09">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Citrobacter_freundii">
        <magnitude><val>283</val></magnitude>
       </node>
       <node name="s__Citrobacter_koseri">
        <magnitude><val>99</val></magnitude>
       </node>
       <node name="s__Citrobacter_portucalensis">
        <magnitude><val>135</val></magnitude>
       </node>
      </node>
      <node name="s__Enterobacteriaceae_endosymbiont_of_Donacia_proxima">
       <magnitude><val>35</val></magnitude>
      </node>
      <node name="g__Plesiomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>123</val></magnitude>
       <node name="s__Plesiomonas_shigelloides">
        <magnitude><val>123</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudocitrobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Pseudocitrobacter_corydidari">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Cedecea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>53</val></magnitude>
       <node name="s__Cedecea_neteri">
        <magnitude><val>53</val></magnitude>
       </node>
      </node>
      <node name="g__Klebsiella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>3873</val></magnitude>
       <node name="s__Klebsiella_variicola">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Klebsiella_pneumoniae">
        <magnitude><val>3642</val></magnitude>
       </node>
       <node name="s__Klebsiella_aerogenes">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Klebsiella_oxytoca">
        <magnitude><val>104</val></magnitude>
       </node>
       <node name="s__Klebsiella_quasipneumoniae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Klebsiella_michiganensis">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Lelliottia">
       <magnitude><val>37</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lelliottia_amnigena">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
      <node name="g__Kluyvera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>79</val></magnitude>
       <node name="s__Kluyvera_cryocrescens">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Kluyvera_ascorbata">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Salmonella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>389</val></magnitude>
       <node name="s__Salmonella_enterica">
        <magnitude><val>389</val></magnitude>
       </node>
      </node>
      <node name="g__Leclercia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>83</val></magnitude>
       <node name="s__Leclercia_adecarboxylata">
        <magnitude><val>83</val></magnitude>
       </node>
      </node>
      <node name="g__Kosakonia">
       <magnitude><val>278</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kosakonia_cowanii">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Kosakonia_oryzendophytica">
        <magnitude><val>220</val></magnitude>
       </node>
       <node name="s__Kosakonia_sacchari">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Cronobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>55</val></magnitude>
       <node name="s__Cronobacter_muytjensii">
        <magnitude><val>55</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Schneideria">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Schneideria_nysicola">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Enterobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>442</val></magnitude>
       <node name="s__Enterobacter_sp._E76">
        <magnitude><val>113</val></magnitude>
       </node>
       <node name="s__Enterobacter_hormaechei">
        <magnitude><val>189</val></magnitude>
       </node>
       <node name="s__Enterobacter_sp._CP102">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Enterobacter_asburiae">
        <magnitude><val>55</val></magnitude>
       </node>
       <node name="s__Enterobacter_cloacae">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Pectobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>337</val></magnitude>
      <node name="g__Pectobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>130</val></magnitude>
       <node name="s__Pectobacterium_wasabiae">
        <magnitude><val>130</val></magnitude>
       </node>
      </node>
      <node name="g__Brenneria">
       <magnitude><val>128</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Brenneria_goodwinii">
        <magnitude><val>115</val></magnitude>
       </node>
       <node name="s__Brenneria_izadpanahii">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Dickeya">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>79</val></magnitude>
       <node name="s__Dickeya_chrysanthemi">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Dickeya_fangzhongdai">
        <magnitude><val>68</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Hafniaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>67</val></magnitude>
      <node name="g__Hafnia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Hafnia_alvei">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Edwardsiella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>44</val></magnitude>
       <node name="s__Edwardsiella_tarda">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Erwiniaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>740</val></magnitude>
      <node name="g__Pantoea">
       <magnitude><val>370</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pantoea_anthophila">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Pantoea_ananatis">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Pantoea_deleyi">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Candidatus_Pantoea_carbekii">
        <magnitude><val>69</val></magnitude>
       </node>
       <node name="s__Pantoea_sp._CCBC3-3-1">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Pantoea_sp._At-9b">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Pantoea_sp._SOD02">
        <magnitude><val>78</val></magnitude>
       </node>
       <node name="s__Pantoea_stewartii">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Tatumella">
       <magnitude><val>24</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tatumella_ptyseos">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Buchnera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>150</val></magnitude>
       <node name="s__Buchnera_aphidicola">
        <magnitude><val>150</val></magnitude>
       </node>
      </node>
      <node name="g__Erwinia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>196</val></magnitude>
       <node name="s__Erwinia_tracheiphila">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Erwinia_billingiae">
        <magnitude><val>88</val></magnitude>
       </node>
       <node name="s__Erwinia_sp._E602">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Erwinia_tasmaniensis">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Candidatus_Erwinia_haradaeae">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bruguierivoracaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>46</val></magnitude>
      <node name="g__Sodalis">
       <magnitude><val>46</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sodalis_ligni">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Yersiniaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>788</val></magnitude>
      <node name="g__Serratia">
       <magnitude><val>173</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Serratia_grimesii">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Serratia_proteamaculans">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Serratia_marcescens">
        <magnitude><val>141</val></magnitude>
       </node>
      </node>
      <node name="g__Rahnella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>420</val></magnitude>
       <node name="s__Rahnella_bonaserana">
        <magnitude><val>335</val></magnitude>
       </node>
       <node name="s__Rahnella_aquatilis">
        <magnitude><val>85</val></magnitude>
       </node>
      </node>
      <node name="g__Yersinia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>185</val></magnitude>
       <node name="s__Yersinia_similis">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Yersinia_kristensenii">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Yersinia_aldovae">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Yersinia_aleksiciae">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Yersinia_hibernica">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Yersinia_alsatica">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Fukatsuia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Candidatus_Fukatsuia_symbiotica">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Budviciaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>144</val></magnitude>
      <node name="g__Pragia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Pragia_fontium">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Leminorella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>69</val></magnitude>
       <node name="s__Leminorella_richardii">
        <magnitude><val>69</val></magnitude>
       </node>
      </node>
      <node name="g__Jinshanibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>47</val></magnitude>
       <node name="s__Jinshanibacter_zhutongyuii">
        <magnitude><val>47</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Morganellaceae">
      <magnitude><val>707</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Providencia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>272</val></magnitude>
       <node name="s__Providencia_heimbachae">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Providencia_alcalifaciens">
        <magnitude><val>261</val></magnitude>
       </node>
      </node>
      <node name="g__Proteus">
       <magnitude><val>257</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Proteus_hauseri">
        <magnitude><val>128</val></magnitude>
       </node>
       <node name="s__Proteus_vulgaris">
        <magnitude><val>115</val></magnitude>
       </node>
       <node name="s__Proteus_mirabilis">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Morganella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>29</val></magnitude>
       <node name="s__Morganella_morganii">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
      <node name="g__Xenorhabdus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>115</val></magnitude>
       <node name="s__Xenorhabdus_griffiniae">
        <magnitude><val>115</val></magnitude>
       </node>
      </node>
      <node name="g__Photorhabdus">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Photorhabdus_asymbiotica">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Methylococcales">
     <magnitude><val>237</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Methylococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>237</val></magnitude>
      <node name="g__Methylomonas">
       <magnitude><val>108</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methylomonas_rhizoryzae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Methylomonas_paludis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Methylomonas_sp._EFPC1">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Methylomonas_denitrificans">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
      <node name="g__Methylotuvimicrobium">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methylotuvimicrobium_buryatense">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Methylococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Methylococcus_geothermalis">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Methylomagnum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>67</val></magnitude>
       <node name="s__Methylomagnum_ishizawai">
        <magnitude><val>67</val></magnitude>
       </node>
      </node>
      <node name="g__Methylomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Methylomicrobium_album">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Methylobacter">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methylobacter_sp._S3L5C">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="g__Candidatus_Thioglobus">
     <magnitude><val>21</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="s__Candidatus_Thioglobus_autotrophicus">
      <magnitude><val>21</val></magnitude>
     </node>
    </node>
    <node name="o__Chromatiales">
     <magnitude><val>429</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Halothiobacillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>16</val></magnitude>
      <node name="g__Halothiobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Halothiobacillus_sp._LS2">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Ectothiorhodospiraceae">
      <magnitude><val>196</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Acidihalobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>144</val></magnitude>
       <node name="s__Acidihalobacter_aeolianus">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Acidihalobacter_yilgarnensis">
        <magnitude><val>134</val></magnitude>
       </node>
      </node>
      <node name="g__Spiribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>52</val></magnitude>
       <node name="s__Spiribacter_curvatus">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Chromatiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>217</val></magnitude>
      <node name="g__Thiocystis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>50</val></magnitude>
       <node name="s__Thiocystis_violascens">
        <magnitude><val>50</val></magnitude>
       </node>
      </node>
      <node name="g__Rheinheimera">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>125</val></magnitude>
       <node name="s__Rheinheimera_sp._F8">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Rheinheimera_sp._MMS21-TC3">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Rheinheimera_sp._MM224">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Nitrosococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Nitrosococcus_wardiae">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Candidatus_Nitrosacidococcus">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Nitrosacidococcus_sp._I8">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Thermochromatium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Thermochromatium_tepidum">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Orbales">
     <magnitude><val>47</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Orbaceae">
      <magnitude><val>47</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gilliamella">
       <magnitude><val>47</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gilliamella_apis">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Gilliamella_sp._ESL0443">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Oceanospirillales">
     <magnitude><val>1395</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hahellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>31</val></magnitude>
      <node name="g__Hahella">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Hahella_sp._HNIBRBA332">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Alcanivoracaceae">
      <magnitude><val>27</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Alloalcanivorax">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27</val></magnitude>
       <node name="s__Alloalcanivorax_xenomutans">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Endozoicomonadaceae">
      <magnitude><val>209</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Endozoicomonas">
       <magnitude><val>209</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Endozoicomonas_sp._GU-1">
        <magnitude><val>114</val></magnitude>
       </node>
       <node name="s__Endozoicomonas_montiporae">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Endozoicomonas_sp._4G">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Endozoicomonas_sp._SCSIO_W0465">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Endozoicomonas_euniceicola">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Endozoicomonas_sp._8E">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Oceanospirillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>788</val></magnitude>
      <node name="g__Marinomonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>50</val></magnitude>
       <node name="s__Marinomonas_sp._CT5">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Marinomonas_sp._GJ51-6">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Marinomonas_mediterranea">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Marinobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Marinobacterium_sediminicola">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Neptunomonas">
       <magnitude><val>241</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Neptunomonas_japonica">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Neptunomonas_concharum">
        <magnitude><val>193</val></magnitude>
       </node>
      </node>
      <node name="g__Neptuniibacter">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Neptuniibacter_halophilus">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Venatoribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25</val></magnitude>
       <node name="s__Venatoribacter_cucullus">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Aliamphritea">
       <magnitude><val>101</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aliamphritea_ceti">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Aliamphritea_hakodatensis">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Bermanella">
       <magnitude><val>346</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Bermanella_marisrubri">
        <magnitude><val>346</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Litorivicinaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>10</val></magnitude>
      <node name="g__Litorivicinus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Litorivicinus_lipolyticus">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Halomonadaceae">
      <magnitude><val>330</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Halomonas">
       <magnitude><val>330</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Halomonas_chromatireducens">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Halomonas_sp._Y3">
        <magnitude><val>219</val></magnitude>
       </node>
       <node name="s__Halomonas_huangheensis">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Halomonas_elongata">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Halomonas_sp._DN3">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Cardiobacteriales">
     <magnitude><val>87</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Cardiobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>53</val></magnitude>
      <node name="g__Suttonella">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Suttonella_sp._R2A3">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
      <node name="g__Cardiobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>22</val></magnitude>
       <node name="s__Cardiobacterium_hominis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Cardiobacterium_sp._Marseille-Q4385">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Ignatzschineriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>34</val></magnitude>
      <node name="g__Ignatzschineria">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>34</val></magnitude>
       <node name="s__Ignatzschineria_rhizosphaerae">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Alteromonadales">
     <magnitude><val>1000</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Idiomarinaceae">
      <magnitude><val>166</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Idiomarina">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>166</val></magnitude>
       <node name="s__Idiomarina_loihiensis">
        <magnitude><val>166</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Pseudoalteromonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>249</val></magnitude>
      <node name="g__Pseudoalteromonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>249</val></magnitude>
       <node name="s__Pseudoalteromonas_distincta">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_spongiae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_piratica">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_sp._MM1">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_espejiana">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_phenolica">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_xiamenensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Pseudoalteromonas_rubra">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Moritellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>23</val></magnitude>
      <node name="g__Moritella">
       <magnitude><val>23</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Moritella_yayanosii">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Psychromonadaceae">
      <magnitude><val>15</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Psychromonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Psychromonas_sp._CNPT3">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Shewanellaceae">
      <magnitude><val>232</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Shewanella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>232</val></magnitude>
       <node name="s__Shewanella_polaris">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Shewanella_halifaxensis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Shewanella_oneidensis">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Shewanella_denitrificans">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Shewanella_sp._MTB7">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Shewanella_sp._ANA-3">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Shewanella_sp._NFH-SH190041">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Shewanella_halotolerans">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Colwelliaceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Colwellia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Colwellia_sp._20A7">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Alteromonadaceae">
      <magnitude><val>302</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Lacimicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Lacimicrobium_alkaliphilum">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Alkalimarinus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>57</val></magnitude>
       <node name="s__Alkalimarinus_coralli">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Alteromonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>192</val></magnitude>
       <node name="s__Alteromonas_macleodii">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Alteromonas_mediterranea">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Alteromonas_sp._76-1">
        <magnitude><val>107</val></magnitude>
       </node>
      </node>
      <node name="g__Catenovulum">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Catenovulum_sediminis">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Salinimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>22</val></magnitude>
       <node name="s__Salinimonas_marina">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="f__Celerinatantimonadaceae">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>32</val></magnitude>
     <node name="g__Celerinatantimonas">
      <magnitude><val>32</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Celerinatantimonas_diazotrophica">
       <magnitude><val>32</val></magnitude>
      </node>
     </node>
    </node>
    <node name="o__Nevskiales">
     <magnitude><val>31</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Steroidobacteraceae">
      <magnitude><val>31</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Steroidobacter">
       <magnitude><val>31</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Steroidobacter_denitrificans">
        <magnitude><val>31</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Campylobacterota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>5831</val></magnitude>
   <node name="c__Epsilonproteobacteria">
    <magnitude><val>5831</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Nautiliales">
     <magnitude><val>207</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Nautiliaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>164</val></magnitude>
      <node name="g__Nautilia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>164</val></magnitude>
       <node name="s__Nautilia_sp._PV-1">
        <magnitude><val>164</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nitratiruptoraceae">
      <magnitude><val>43</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nitrosophilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>43</val></magnitude>
       <node name="s__Nitrosophilus_alvini">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Campylobacterales">
     <magnitude><val>5624</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Sulfurospirillaceae">
      <magnitude><val>98</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Sulfurospirillum">
       <magnitude><val>98</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sulfurospirillum_multivorans">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Sulfurospirillum_cavolei">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Sulfurospirillum_halorespirans">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sulfurovaceae">
      <magnitude><val>103</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Sulfurovum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>103</val></magnitude>
       <node name="s__Sulfurovum_mangrovi">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Sulfurovum_indicum">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Helicobacteraceae">
      <magnitude><val>203</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Helicobacter">
       <magnitude><val>203</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Helicobacter_pylori">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Helicobacter_cholecystus">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Helicobacter_canadensis">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Helicobacter_pullorum">
        <magnitude><val>53</val></magnitude>
       </node>
       <node name="s__Helicobacter_sp._NHP21005">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Helicobacter_winghamensis">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Arcobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>405</val></magnitude>
      <node name="g__Aliarcobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>318</val></magnitude>
       <node name="s__Aliarcobacter_butzleri">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Aliarcobacter_cryaerophilus">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Aliarcobacter_faecis">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Aliarcobacter_thereius">
        <magnitude><val>272</val></magnitude>
       </node>
      </node>
      <node name="g__Malaciobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Malaciobacter_molluscorum">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Arcobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>44</val></magnitude>
       <node name="s__Arcobacter_porcinus">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
      <node name="g__Halarcobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Halarcobacter_anaerophilus">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Campylobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>4471</val></magnitude>
      <node name="g__Campylobacter">
       <magnitude><val>4471</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Campylobacter_sp._VBCF_01_NA2">
        <magnitude><val>95</val></magnitude>
       </node>
       <node name="s__Campylobacter_corcagiensis">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Campylobacter_blaseri">
        <magnitude><val>64</val></magnitude>
       </node>
       <node name="s__Campylobacter_concisus">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Campylobacter_coli">
        <magnitude><val>270</val></magnitude>
       </node>
       <node name="s__Campylobacter_sputorum">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Campylobacter_pinnipediorum">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Campylobacter_showae">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Campylobacter_ureolyticus">
        <magnitude><val>526</val></magnitude>
       </node>
       <node name="s__Campylobacter_sp._RM6914">
        <magnitude><val>339</val></magnitude>
       </node>
       <node name="s__Campylobacter_canadensis">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Campylobacter_sp._RM16187">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Campylobacter_jejuni">
        <magnitude><val>2572</val></magnitude>
       </node>
       <node name="s__Campylobacter_novaezeelandiae">
        <magnitude><val>414</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Sulfurimonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>344</val></magnitude>
      <node name="g__Sulfurimonas">
       <magnitude><val>208</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sulfurimonas_sediminis">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Sulfurimonas_gotlandica">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Sulfurimonas_lithotrophica">
        <magnitude><val>91</val></magnitude>
       </node>
       <node name="s__Sulfurimonas_paralvinellae">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Sulfurimonas_marina">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Sulfuricurvum">
       <magnitude><val>136</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sulfuricurvum_kujiense">
        <magnitude><val>136</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Kiritimatiellota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>62</val></magnitude>
   <node name="c__Tichowtungiia">
    <magnitude><val>16</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Tichowtungiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>16</val></magnitude>
     <node name="f__Tichowtungiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>16</val></magnitude>
      <node name="g__Tichowtungia">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tichowtungia_aerotolerans">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Kiritimatiellia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>46</val></magnitude>
    <node name="o__Kiritimatiellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>46</val></magnitude>
     <node name="f__Kiritimatiellaceae">
      <magnitude><val>46</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Kiritimatiella">
       <magnitude><val>46</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kiritimatiella_glycovorans">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Acidobacteriota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>841</val></magnitude>
   <node name="c__Blastocatellia">
    <magnitude><val>80</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="g__Chloracidobacterium">
     <magnitude><val>80</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="s__Chloracidobacterium_aggregatum">
      <magnitude><val>80</val></magnitude>
     </node>
    </node>
   </node>
   <node name="c__Vicinamibacteria">
    <magnitude><val>18</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Vicinamibacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>18</val></magnitude>
     <node name="f__Vicinamibacteraceae">
      <magnitude><val>18</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Luteitalea">
       <magnitude><val>18</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Luteitalea_pratensis">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Terriglobia">
    <magnitude><val>641</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Terriglobales">
     <magnitude><val>585</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Acidobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>585</val></magnitude>
      <node name="g__Candidatus_Koribacter">
       <magnitude><val>315</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Koribacter_versatilis">
        <magnitude><val>315</val></magnitude>
       </node>
      </node>
      <node name="g__Alloacidobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Alloacidobacterium_dinghuense">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Occallatibacter">
       <magnitude><val>17</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Occallatibacter_riparius">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Terriglobus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>66</val></magnitude>
       <node name="s__Terriglobus_roseus">
        <magnitude><val>66</val></magnitude>
       </node>
      </node>
      <node name="g__Edaphobacter">
       <magnitude><val>174</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Edaphobacter_lichenicola">
        <magnitude><val>140</val></magnitude>
       </node>
       <node name="s__Edaphobacter_sp._12200R-103">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Edaphobacter_sp._4G125">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Bryobacterales">
     <magnitude><val>56</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Bryobacteraceae">
      <magnitude><val>56</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Paludibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>56</val></magnitude>
       <node name="s__Paludibaculum_fermentans">
        <magnitude><val>56</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Holophagae">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>102</val></magnitude>
    <node name="o__Thermotomaculales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>41</val></magnitude>
     <node name="f__Thermotomaculaceae">
      <magnitude><val>41</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermotomaculum">
       <magnitude><val>41</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermotomaculum_hydrothermale">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Holophagales">
     <magnitude><val>50</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Holophagaceae">
      <magnitude><val>50</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Geothrix">
       <magnitude><val>50</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Geothrix_oryzae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Geothrix_sp._PMB-07">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Acanthopleuribacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11</val></magnitude>
     <node name="f__Acanthopleuribacteraceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Sulfidibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Sulfidibacter_corallicola">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Gemmatimonadota">
   <magnitude><val>103</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Gemmatimonadetes">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>103</val></magnitude>
    <node name="o__Gemmatimonadales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>103</val></magnitude>
     <node name="f__Gemmatimonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>103</val></magnitude>
      <node name="g__Gemmatimonas">
       <magnitude><val>103</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gemmatimonas_phototrophica">
        <magnitude><val>103</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Thermodesulfobacteriota">
   <magnitude><val>10332</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Thermodesulfobacteria">
    <magnitude><val>44</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Thermodesulfobacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>44</val></magnitude>
     <node name="f__Thermodesulfobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>44</val></magnitude>
      <node name="g__Thermodesulfobacterium">
       <magnitude><val>23</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermodesulfobacterium_geofontis">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Thermosulfurimonas">
       <magnitude><val>21</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermosulfurimonas_marina">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfobulbia">
    <magnitude><val>371</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Desulfobulbales">
     <magnitude><val>371</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Desulfobulbaceae">
      <magnitude><val>167</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfogranum">
       <magnitude><val>18</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfogranum_marinum">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfurivibrio">
       <magnitude><val>24</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfurivibrio_alkaliphilus">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfobulbus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>87</val></magnitude>
       <node name="s__Desulfobulbus_oralis">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Desulfobulbus_propionicus">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Desulfobulbus_oligotrophicus">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__uncultured_Desulfobulbus_sp.">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfolithobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Desulfolithobacter_dissulfuricans">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfomarina">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Desulfomarina_profundi">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfocapsaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>204</val></magnitude>
      <node name="g__Desulfosediminicola">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Desulfosediminicola_ganghwensis">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfopila">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>134</val></magnitude>
       <node name="s__Desulfopila_sp._IMCC35008">
        <magnitude><val>134</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfofustis">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Desulfofustis_limnaeus">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfotalea">
       <magnitude><val>35</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfotalea_psychrophila">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Syntrophia">
    <magnitude><val>16</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Syntrophales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>16</val></magnitude>
     <node name="f__Syntrophaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>16</val></magnitude>
      <node name="g__Syntrophus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Syntrophus_aciditrophicus">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfobacteria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>789</val></magnitude>
    <node name="o__Desulfobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>789</val></magnitude>
     <node name="f__Desulfosudaceae">
      <magnitude><val>26</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfosudis">
       <magnitude><val>26</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfosudis_oleivorans">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfolunaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>96</val></magnitude>
      <node name="g__Desulfoluna">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>96</val></magnitude>
       <node name="s__Desulfoluna_limicola">
        <magnitude><val>96</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfobacteraceae">
      <magnitude><val>452</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfobacter">
       <magnitude><val>441</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Desulfobacter_sp.">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Desulfobacter_postgatei">
        <magnitude><val>386</val></magnitude>
       </node>
       <node name="s__Desulfobacter_hydrogenophilus">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Desulforapulum">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulforapulum_autotrophicum">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfococcaceae">
      <magnitude><val>86</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>51</val></magnitude>
       <node name="s__Desulfococcus_multivorans">
        <magnitude><val>51</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfonema">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>35</val></magnitude>
       <node name="s__Desulfonema_magnum">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Desulfonema_limicola">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfosarcinaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>129</val></magnitude>
      <node name="g__Desulfosarcina">
       <magnitude><val>129</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfosarcina_ovata">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__uncultured_Desulfosarcina_sp.">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Desulfosarcina_alkanivorans">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Desulfosarcina_widdelii">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Desulfosarcina_sp._BuS5">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfomonilia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>17</val></magnitude>
    <node name="o__Desulfomonilales">
     <magnitude><val>17</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Desulfomonilaceae">
      <magnitude><val>17</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfomonile">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Desulfomonile_tiedjei">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfuromonadia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>631</val></magnitude>
    <node name="o__Desulfuromonadales">
     <magnitude><val>290</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Syntrophotaleaceae">
      <magnitude><val>227</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Syntrophotalea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>227</val></magnitude>
       <node name="s__Syntrophotalea_acetylenivorans">
        <magnitude><val>77</val></magnitude>
       </node>
       <node name="s__Syntrophotalea_acetylenica">
        <magnitude><val>138</val></magnitude>
       </node>
       <node name="s__Syntrophotalea_carbinolica">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfuromonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>48</val></magnitude>
      <node name="g__Pelobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Pelobacter_propionicus">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfuromonas">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfuromonas_versatilis">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Geoalkalibacteraceae">
      <magnitude><val>15</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Geoalkalibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Geoalkalibacter_subterraneus">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Geobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>341</val></magnitude>
     <node name="f__Geobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>341</val></magnitude>
      <node name="g__Citrifermentans">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>24</val></magnitude>
       <node name="s__Citrifermentans_bremense">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Geomonas">
       <magnitude><val>99</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Geomonas_paludis">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Geomonas_sp._RF6">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Geomonas_subterranea">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Geobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>143</val></magnitude>
       <node name="s__Geobacter_metallireducens">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Geobacter_sp._FeAm09">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Geobacter_sp._SVR">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Geobacter_sp._DSM_9736">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Geobacter_benzoatilyticus">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Geobacter_sulfurreducens">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Trichlorobacter">
       <magnitude><val>37</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Trichlorobacter_lovleyi">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
      <node name="g__Geotalea">
       <magnitude><val>38</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Geotalea_uraniireducens">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfarculia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>18</val></magnitude>
    <node name="o__Desulfarculales">
     <magnitude><val>18</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Desulfarculaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>18</val></magnitude>
      <node name="g__Desulfarculus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Desulfarculus_baarsii">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Syntrophobacteria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>33</val></magnitude>
    <node name="o__Syntrophobacterales">
     <magnitude><val>33</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Syntrophobacteraceae">
      <magnitude><val>33</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Syntrophobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Syntrophobacter_fumaroxidans">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Candidatus_Desulfofervidia">
    <magnitude><val>15</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Candidatus_Desulfofervidales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>15</val></magnitude>
     <node name="f__Candidatus_Desulfofervidaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>15</val></magnitude>
      <node name="g__Candidatus_Desulfofervidus">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Desulfofervidus_auxilii">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Desulfovibrionia">
    <magnitude><val>8398</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Desulfovibrionales">
     <magnitude><val>8398</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Desulfovibrionaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>8120</val></magnitude>
      <node name="g__Desulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>4029</val></magnitude>
       <node name="s__Desulfovibrio_vulgaris">
        <magnitude><val>752</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_subterraneus">
        <magnitude><val>542</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_fairfieldensis">
        <magnitude><val>396</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_mangrovi">
        <magnitude><val>157</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_desulfuricans">
        <magnitude><val>699</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_sp._G11">
        <magnitude><val>440</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_ferrophilus">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Candidatus_Desulfovibrio_trichonymphae">
        <magnitude><val>49</val></magnitude>
       </node>
       <node name="s__Desulfovibrio_piger">
        <magnitude><val>965</val></magnitude>
       </node>
      </node>
      <node name="g__Oleidesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>451</val></magnitude>
       <node name="s__Oleidesulfovibrio_alaskensis">
        <magnitude><val>451</val></magnitude>
       </node>
      </node>
      <node name="g__Cupidesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>835</val></magnitude>
       <node name="s__Cupidesulfovibrio_liaohensis">
        <magnitude><val>835</val></magnitude>
       </node>
      </node>
      <node name="g__Oceanidesulfovibrio">
       <magnitude><val>118</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Oceanidesulfovibrio_marinus">
        <magnitude><val>118</val></magnitude>
       </node>
      </node>
      <node name="g__Paradesulfovibrio_(ex_Waite_et_al._2020)">
       <magnitude><val>35</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paradesulfovibrio_bizertensis">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfocurvibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Desulfocurvibacter_africanus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Solidesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>259</val></magnitude>
       <node name="s__Solidesulfovibrio_magneticus">
        <magnitude><val>146</val></magnitude>
       </node>
       <node name="s__Solidesulfovibrio_carbinolicus">
        <magnitude><val>63</val></magnitude>
       </node>
       <node name="s__Solidesulfovibrio_carbinoliphilus">
        <magnitude><val>50</val></magnitude>
       </node>
      </node>
      <node name="g__Salidesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>159</val></magnitude>
       <node name="s__Salidesulfovibrio_onnuriiensis">
        <magnitude><val>159</val></magnitude>
       </node>
      </node>
      <node name="g__Maridesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>549</val></magnitude>
       <node name="s__Maridesulfovibrio_salexigens">
        <magnitude><val>131</val></magnitude>
       </node>
       <node name="s__Maridesulfovibrio_hydrothermalis">
        <magnitude><val>418</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfolutivibrio">
       <magnitude><val>157</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Desulfolutivibrio_sulfoxidireducens">
        <magnitude><val>95</val></magnitude>
       </node>
       <node name="s__Desulfolutivibrio_sulfodismutans">
        <magnitude><val>62</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudodesulfovibrio">
       <magnitude><val>1053</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Pseudodesulfovibrio_sp.">
        <magnitude><val>252</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_tunisiensis">
        <magnitude><val>82</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_nedwellii">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_sediminis">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_profundus">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_portus">
        <magnitude><val>57</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_thermohalotolerans">
        <magnitude><val>70</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_indicus">
        <magnitude><val>151</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_sp._zrk46">
        <magnitude><val>76</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_mercurii">
        <magnitude><val>142</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_cashew">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Pseudodesulfovibrio_aespoeensis">
        <magnitude><val>71</val></magnitude>
       </node>
      </node>
      <node name="g__Lawsonia">
       <magnitude><val>298</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lawsonia_intracellularis">
        <magnitude><val>298</val></magnitude>
       </node>
      </node>
      <node name="g__Megalodesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>151</val></magnitude>
       <node name="s__Megalodesulfovibrio_gigas">
        <magnitude><val>151</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfomicrobiaceae">
      <magnitude><val>251</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermodesulfomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>65</val></magnitude>
       <node name="s__Thermodesulfomicrobium_sp._WS">
        <magnitude><val>65</val></magnitude>
       </node>
      </node>
      <node name="g__Desulfomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>186</val></magnitude>
       <node name="s__Desulfomicrobium_sp._ZS1">
        <magnitude><val>72</val></magnitude>
       </node>
       <node name="s__Desulfomicrobium_orale">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Desulfomicrobium_baculatum">
        <magnitude><val>56</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Desulfohalobiaceae">
      <magnitude><val>27</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Desulfohalobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27</val></magnitude>
       <node name="s__Desulfohalobium_retbaense">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Candidatus_Saccharibacteria">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>444</val></magnitude>
   <node name="g__Candidatus_Minimicrobia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>39</val></magnitude>
    <node name="s__Candidatus_Minimicrobia_vallesae">
     <magnitude><val>39</val></magnitude>
    </node>
   </node>
   <node name="c__Candidatus_Saccharimonadia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>405</val></magnitude>
    <node name="o__Candidatus_Nanosynbacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>405</val></magnitude>
     <node name="f__Candidatus_Nanosynbacteraceae">
      <magnitude><val>405</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Nanosynbacter">
       <magnitude><val>405</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Nanosynbacter_lyticus">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Candidatus_Nanosynbacter_sp._HMT-352">
        <magnitude><val>367</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Chloroflexota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>251</val></magnitude>
   <node name="c__Ardenticatenia">
    <magnitude><val>22</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Candidatus_Promineifilales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>22</val></magnitude>
     <node name="f__Candidatus_Promineifilaceae">
      <magnitude><val>22</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candidatus_Promineifilum">
       <magnitude><val>22</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Promineifilum_breve">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Dehalococcoidia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>61</val></magnitude>
    <node name="o__Dehalococcoidales">
     <magnitude><val>61</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Dehalococcoidaceae">
      <magnitude><val>61</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Dehalococcoides">
       <magnitude><val>61</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dehalococcoides_mccartyi">
        <magnitude><val>61</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Anaerolineae">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>53</val></magnitude>
    <node name="o__Anaerolineales">
     <magnitude><val>53</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Anaerolineaceae">
      <magnitude><val>53</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pelolinea">
       <magnitude><val>39</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pelolinea_submarina">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
      <node name="g__Anaerolinea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Anaerolinea_thermophila">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Ktedonobacteria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>80</val></magnitude>
    <node name="o__Ktedonobacterales">
     <magnitude><val>80</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Ktedonosporobacteraceae">
      <magnitude><val>80</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Ktedonosporobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>80</val></magnitude>
       <node name="s__Ktedonosporobacter_rubrisoli">
        <magnitude><val>80</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Chloroflexia">
    <magnitude><val>24</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Chloroflexales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>24</val></magnitude>
     <node name="f__Chloroflexaceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Chloroflexus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Chloroflexus_aurantiacus">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Roseiflexaceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Roseiflexus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Roseiflexus_castenholzii">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Caldilineae">
    <magnitude><val>11</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Caldilineales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11</val></magnitude>
     <node name="f__Caldilineaceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Caldilinea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Caldilinea_aerophila">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="s__unidentified_bacterial_endosymbiont">
   <magnitude><val>13</val></magnitude>
  </node>
  <node name="p__Chlamydiota">
   <magnitude><val>141</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Chlamydiia">
    <magnitude><val>141</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Chlamydiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>121</val></magnitude>
     <node name="f__Chlamydiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>121</val></magnitude>
      <node name="g__Chlamydia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>121</val></magnitude>
       <node name="s__Chlamydia_muridarum">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Candidatus_Chlamydia_sanziniae">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Chlamydia_pecorum">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Chlamydia_poikilotherma">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Parachlamydiales">
     <magnitude><val>20</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Rhabdochlamydiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>20</val></magnitude>
      <node name="g__Candidatus_Rhabdochlamydia">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Rhabdochlamydia_porcellionis">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Actinomycetota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>1474368</val></magnitude>
   <node name="c__Coriobacteriia">
    <magnitude><val>781796</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Coriobacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>3180</val></magnitude>
     <node name="f__Atopobiaceae">
      <magnitude><val>991</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Parolsenella">
       <magnitude><val>388</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parolsenella_catena">
        <magnitude><val>317</val></magnitude>
       </node>
       <node name="s__Parolsenella_massiliensis">
        <magnitude><val>71</val></magnitude>
       </node>
      </node>
      <node name="g__Leptogranulimonas">
       <magnitude><val>260</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leptogranulimonas_caecicola">
        <magnitude><val>260</val></magnitude>
       </node>
      </node>
      <node name="g__Parafannyhessea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Parafannyhessea_umbonata">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Lancefieldella">
       <magnitude><val>126</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lancefieldella_sp._Marseille-Q7238">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Lancefieldella_parvula">
        <magnitude><val>110</val></magnitude>
       </node>
      </node>
      <node name="g__Fannyhessea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>42</val></magnitude>
       <node name="s__Fannyhessea_vaginae">
        <magnitude><val>42</val></magnitude>
       </node>
      </node>
      <node name="g__Olsenella">
       <magnitude><val>100</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Olsenella_sp._oral_taxon_807">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Olsenella_uli">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Olsenella_timonensis">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Thermophilibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>30</val></magnitude>
       <node name="s__Thermophilibacter_immobilis">
        <magnitude><val>30</val></magnitude>
       </node>
      </node>
      <node name="g__Atopobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>35</val></magnitude>
       <node name="s__Atopobium_sp._oral_taxon_416">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Coriobacteriaceae">
      <magnitude><val>2189</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Collinsella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2161</val></magnitude>
       <node name="s__Collinsella_sp._zg1085">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Collinsella_aerofaciens">
        <magnitude><val>2055</val></magnitude>
       </node>
       <node name="s__Collinsella_stercoris">
        <magnitude><val>62</val></magnitude>
       </node>
      </node>
      <node name="g__Coriobacterium">
       <magnitude><val>28</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Coriobacterium_glomerans">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Eggerthellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>778616</val></magnitude>
     <node name="f__Eggerthellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>778616</val></magnitude>
      <node name="g__Gordonibacter">
       <magnitude><val>82652</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gordonibacter_pamelaeae">
        <magnitude><val>74815</val></magnitude>
       </node>
       <node name="s__Gordonibacter_urolithinfaciens">
        <magnitude><val>7837</val></magnitude>
       </node>
      </node>
      <node name="g__Slackia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>60</val></magnitude>
       <node name="s__Slackia_heliotrinireducens">
        <magnitude><val>60</val></magnitude>
       </node>
      </node>
      <node name="g__Berryella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>117</val></magnitude>
       <node name="s__Berryella_intestinalis">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Berryella_wangjianweii">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Raoultibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>112</val></magnitude>
       <node name="s__Raoultibacter_timonensis">
        <magnitude><val>112</val></magnitude>
       </node>
      </node>
      <node name="g__Cryptobacterium">
       <magnitude><val>122</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cryptobacterium_curtum">
        <magnitude><val>122</val></magnitude>
       </node>
      </node>
      <node name="g__Phoenicibacter">
       <magnitude><val>137</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Phoenicibacter_congonensis">
        <magnitude><val>137</val></magnitude>
       </node>
      </node>
      <node name="g__Denitrobacterium">
       <magnitude><val>41</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Denitrobacterium_detoxificans">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Eggerthella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>442450</val></magnitude>
       <node name="s__Eggerthella_guodeyinii">
        <magnitude><val>1380</val></magnitude>
       </node>
       <node name="s__Eggerthella_sp._YY7918">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Eggerthella_lenta">
        <magnitude><val>441011</val></magnitude>
       </node>
      </node>
      <node name="g__Adlercreutzia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>252535</val></magnitude>
       <node name="s__Adlercreutzia_hattorii">
        <magnitude><val>202729</val></magnitude>
       </node>
       <node name="s__Adlercreutzia_equolifaciens">
        <magnitude><val>49806</val></magnitude>
       </node>
      </node>
      <node name="g__Xiamenia">
       <magnitude><val>99</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Xiamenia_xianingshaonis">
        <magnitude><val>99</val></magnitude>
       </node>
      </node>
      <node name="g__Arabiibacter">
       <magnitude><val>291</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Arabiibacter_massiliensis">
        <magnitude><val>291</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Rubrobacteria">
    <magnitude><val>13</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Rubrobacterales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>13</val></magnitude>
     <node name="f__Rubrobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>13</val></magnitude>
      <node name="g__Rubrobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Rubrobacter_xylanophilus">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Actinomycetes">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>692441</val></magnitude>
    <node name="o__Geodermatophilales">
     <magnitude><val>11</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Geodermatophilaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>11</val></magnitude>
      <node name="g__Blastococcus">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Blastococcus_saxobsidens">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Candidatus_Nanopelagicales">
     <magnitude><val>47</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Candidatus_Nanopelagicaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>47</val></magnitude>
      <node name="g__Candidatus_Planktophila">
       <magnitude><val>47</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Planktophila_lacus">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Candidatus_Planktophila_dulcis">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Candidatus_Planktophila_sulfonica">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Streptosporangiales">
     <magnitude><val>130</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Streptosporangiaceae">
      <magnitude><val>36</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermobispora">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermobispora_bispora">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Nonomuraea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25</val></magnitude>
       <node name="s__Nonomuraea_coxensis">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nocardiopsaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>77</val></magnitude>
      <node name="g__Nocardiopsis">
       <magnitude><val>77</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nocardiopsis_exhalans">
        <magnitude><val>77</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermomonosporaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>17</val></magnitude>
      <node name="g__Thermomonospora">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Thermomonospora_amylolytica">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Pseudonocardiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>229</val></magnitude>
     <node name="f__Pseudonocardiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>229</val></magnitude>
      <node name="g__Kutzneria">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kutzneria_chonburiensis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Saccharopolyspora">
       <magnitude><val>25</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Saccharopolyspora_pogona">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Actinosynnema">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Actinosynnema_mirum">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Amycolatopsis">
       <magnitude><val>113</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Amycolatopsis_sp._FDAARGOS_1241">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Amycolatopsis_sp._CA-230715">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Amycolatopsis_sp._HUAS_11-8">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Amycolatopsis_sp._AA4">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Amycolatopsis_aidingensis">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Amycolatopsis_albispora">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudonocardia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>33</val></magnitude>
       <node name="s__Pseudonocardia_broussonetiae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Pseudonocardia_sp._DSM_110487">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Lentzea">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lentzea_sp._HUAS12">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Nakamurellales">
     <magnitude><val>36</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Nakamurellaceae">
      <magnitude><val>36</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nakamurella">
       <magnitude><val>36</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nakamurella_sp._PAMC28650">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Nakamurella_multipartita">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Bifidobacteriales">
     <magnitude><val>651274</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Bifidobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>651274</val></magnitude>
      <node name="g__Gardnerella">
       <magnitude><val>475</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gardnerella_vaginalis">
        <magnitude><val>475</val></magnitude>
       </node>
      </node>
      <node name="g__Bifidobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>650774</val></magnitude>
       <node name="s__Bifidobacterium_sp._KimH">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_saguini">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_scardovii">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_thermophilum">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_asteroides">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_breve">
        <magnitude><val>6260</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_eulemuris">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_longum">
        <magnitude><val>636015</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_sp._ESL0704">
        <magnitude><val>86</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_adolescentis">
        <magnitude><val>6782</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_catenulatum">
        <magnitude><val>576</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_subtile">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_choerinum">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_sp._ESL0690">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_actinocoloniiforme">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_sp._ESL0732">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_pseudolongum">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_pseudocatenulatum">
        <magnitude><val>188</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_pullorum">
        <magnitude><val>104</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_sp._ESL0769">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_dentium">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_animalis">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_angulatum">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_imperatoris">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Bifidobacterium_bifidum">
        <magnitude><val>90</val></magnitude>
       </node>
      </node>
      <node name="g__Parascardovia">
       <magnitude><val>25</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parascardovia_denticolens">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Micromonosporales">
     <magnitude><val>117</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Micromonosporaceae">
      <magnitude><val>117</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Actinoplanes">
       <magnitude><val>58</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Actinoplanes_ianthinogenes">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Actinoplanes_sp._N902-109">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Polymorphospora">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Polymorphospora_rubra">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Phytohabitans">
       <magnitude><val>18</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Phytohabitans_suffuscus">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Dactylosporangium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25</val></magnitude>
       <node name="s__Dactylosporangium_roseum">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Catenulisporales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>13</val></magnitude>
     <node name="f__Catenulisporaceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Catenulispora">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Catenulispora_acidiphila">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Micrococcales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>2246</val></magnitude>
     <node name="f__Brevibacteriaceae">
      <magnitude><val>58</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Brevibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>58</val></magnitude>
       <node name="s__Brevibacterium_siliguriense">
        <magnitude><val>58</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Microbacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>366</val></magnitude>
      <node name="g__Leucobacter">
       <magnitude><val>41</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leucobacter_insecticola">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Leucobacter_triazinivorans">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Leucobacter_luti">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Agromyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__Agromyces_sp._H17E-10">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodoluna">
       <magnitude><val>27</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Rhodoluna_planktonica">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Microbacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>178</val></magnitude>
       <node name="s__Microbacterium_sp._zg-B185">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Microbacterium_amylolyticum">
        <magnitude><val>107</val></magnitude>
       </node>
      </node>
      <node name="g__Aquiluna">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Aquiluna_borgnonia">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Curtobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Curtobacterium_flaccumfaciens">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Cryobacterium">
       <magnitude><val>37</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cryobacterium_breve">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Promicromonosporaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>322</val></magnitude>
      <node name="g__Isoptericola">
       <magnitude><val>322</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Isoptericola_variabilis">
        <magnitude><val>322</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Micrococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1459</val></magnitude>
      <node name="g__Rothia">
       <magnitude><val>499</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Rothia_mucilaginosa">
        <magnitude><val>193</val></magnitude>
       </node>
       <node name="s__Rothia_aeria">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Rothia_dentocariosa">
        <magnitude><val>269</val></magnitude>
       </node>
      </node>
      <node name="g__Renibacterium">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Renibacterium_salmoninarum">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Glutamicibacter">
       <magnitude><val>126</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Glutamicibacter_halophytocola">
        <magnitude><val>126</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudarthrobacter">
       <magnitude><val>100</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudarthrobacter_sp._NIBRBAC000502770">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Pseudarthrobacter_sp._L1SW">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Micrococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>37</val></magnitude>
       <node name="s__Micrococcus_lylae">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Micrococcus_terreus">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Arthrobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>682</val></magnitude>
       <node name="s__Arthrobacter_zhangbolii">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sp._NEB_688">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Arthrobacter_crystallopoietes">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sp._Y-9">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sp._Helios">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Arthrobacter_gengyunqii">
        <magnitude><val>130</val></magnitude>
       </node>
       <node name="s__Arthrobacter_agilis">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sp._NicSoilC5">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sp._QXT-31">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Arthrobacter_sunyaminii">
        <magnitude><val>351</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Dermabacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>41</val></magnitude>
      <node name="g__Helcobacillus">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Helcobacillus_massiliensis">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Brachybacterium">
       <magnitude><val>30</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Brachybacterium_huguangmaarense">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Brachybacterium_sp._P6-10-X1">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Propionibacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>362</val></magnitude>
     <node name="f__Propionibacteriaceae">
      <magnitude><val>273</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Propionibacterium">
       <magnitude><val>53</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Propionibacterium_acidifaciens">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Propionibacterium_freudenreichii">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Propionimicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>16</val></magnitude>
       <node name="s__Propionimicrobium_sp._PCR01-08-3">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Cutibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Cutibacterium_acnes">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Arachnia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>119</val></magnitude>
       <node name="s__Arachnia_propionica">
        <magnitude><val>106</val></magnitude>
       </node>
       <node name="s__Arachnia_rubra">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Vaginimicrobium">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Vaginimicrobium_propionicum">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Tessaracoccus">
       <magnitude><val>54</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tessaracoccus_flavescens">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Tessaracoccus_defluvii">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nocardioidaceae">
      <magnitude><val>89</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pimelobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>27</val></magnitude>
       <node name="s__Pimelobacter_simplex">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Nocardioides">
       <magnitude><val>62</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nocardioides_ochotonae">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Nocardioides_sp._cx-173">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Jatrophihabitantales">
     <magnitude><val>21</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Jatrophihabitantaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>21</val></magnitude>
      <node name="g__Jatrophihabitans">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Jatrophihabitans_telluris">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Mycobacteriales">
     <magnitude><val>3784</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Lawsonellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>20</val></magnitude>
      <node name="g__Lawsonella">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lawsonella_clevelandensis">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nocardiaceae">
      <magnitude><val>741</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nocardia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>139</val></magnitude>
       <node name="s__Nocardia_terpenica">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Nocardia_brasiliensis">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Nocardia_sputorum">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Nocardia_cyriacigeorgica">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Nocardia_asteroides">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Rhodococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>602</val></magnitude>
       <node name="s__Rhodococcus_pyridinivorans">
        <magnitude><val>569</val></magnitude>
       </node>
       <node name="s__Rhodococcus_opacus">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Rhodococcus_sp._SGAir0479">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Gordoniaceae">
      <magnitude><val>43</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Gordonia">
       <magnitude><val>43</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Gordonia_sp._NB41Y">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Gordonia_sp._X0973">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Corynebacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1778</val></magnitude>
      <node name="g__Corynebacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1778</val></magnitude>
       <node name="s__Corynebacterium_tuberculostearicum">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Corynebacterium_kroppenstedtii">
        <magnitude><val>524</val></magnitude>
       </node>
       <node name="s__Corynebacterium_pseudopelargi">
        <magnitude><val>65</val></magnitude>
       </node>
       <node name="s__Corynebacterium_glucuronolyticum">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Corynebacterium_endometrii">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Corynebacterium_durum">
        <magnitude><val>145</val></magnitude>
       </node>
       <node name="s__Corynebacterium_aquilae">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Corynebacterium_striatum">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Corynebacterium_pseudotuberculosis">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Corynebacterium_camporealensis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Corynebacterium_jeikeium">
        <magnitude><val>50</val></magnitude>
       </node>
       <node name="s__Corynebacterium_glutamicum">
        <magnitude><val>140</val></magnitude>
       </node>
       <node name="s__Corynebacterium_pyruviciproducens">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Corynebacterium_falsenii">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Corynebacterium_accolens">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Corynebacterium_simulans">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Corynebacterium_freiburgense">
        <magnitude><val>125</val></magnitude>
       </node>
       <node name="s__Corynebacterium_kutscheri">
        <magnitude><val>58</val></magnitude>
       </node>
       <node name="s__Corynebacterium_hindlerae">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Corynebacterium_occultum">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Corynebacterium_rouxii">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Corynebacterium_macginleyi">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Corynebacterium_diphtheriae">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Corynebacterium_minutissimum">
        <magnitude><val>261</val></magnitude>
       </node>
       <node name="s__Corynebacterium_pseudodiphtheriticum">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Corynebacterium_lujinxingii">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Corynebacterium_riegelii">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Segniliparaceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Segniliparus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Segniliparus_rotundus">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Mycobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>1175</val></magnitude>
      <node name="g__Mycobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>922</val></magnitude>
       <node name="s__Mycobacterium_paragordonae">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Mycobacterium_gallinarum">
        <magnitude><val>35</val></magnitude>
       </node>
       <node name="s__Mycobacterium_sp._ITM-2016-00318">
        <magnitude><val>449</val></magnitude>
       </node>
       <node name="s__Mycobacterium_sp._IDR2000157661">
        <magnitude><val>375</val></magnitude>
       </node>
       <node name="s__Mycobacterium_malmoense">
        <magnitude><val>42</val></magnitude>
       </node>
      </node>
      <node name="g__Mycolicibacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>228</val></magnitude>
       <node name="s__Mycolicibacterium_neoaurum">
        <magnitude><val>44</val></magnitude>
       </node>
       <node name="s__Mycolicibacterium_crocinum">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Mycolicibacterium_hassiacum">
        <magnitude><val>129</val></magnitude>
       </node>
       <node name="s__Mycolicibacterium_sp._YH-1">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Mycolicibacterium_madagascariense">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Mycobacteroides">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25</val></magnitude>
       <node name="s__Mycobacteroides_chelonae">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Mycobacteroides_abscessus">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Dietziaceae">
      <magnitude><val>16</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Dietzia">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Dietzia_sp._B32">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Actinomycetales">
     <magnitude><val>33200</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Actinomycetaceae">
      <magnitude><val>33200</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Actinomyces">
       <magnitude><val>7249</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Actinomyces_massiliensis">
        <magnitude><val>234</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._oral_taxon_171">
        <magnitude><val>1057</val></magnitude>
       </node>
       <node name="s__Actinomyces_howellii">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Actinomyces_oris">
        <magnitude><val>1678</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._HMT_175">
        <magnitude><val>422</val></magnitude>
       </node>
       <node name="s__Actinomyces_viscosus">
        <magnitude><val>127</val></magnitude>
       </node>
       <node name="s__Actinomyces_capricornis">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._oral_taxon_169">
        <magnitude><val>1896</val></magnitude>
       </node>
       <node name="s__Actinomyces_naeslundii">
        <magnitude><val>560</val></magnitude>
       </node>
       <node name="s__Actinomyces_lilanjuaniae">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._zg-332">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Actinomyces_pacaensis">
        <magnitude><val>1105</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._Chiba101">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Actinomyces_sp._oral_taxon_414">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Actinomyces_slackii">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Actinomyces_israelii">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Arcanobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Arcanobacterium_phocae">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Gleimia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Gleimia_europaea">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Winkia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Winkia_neuii">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Changpingibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Changpingibacter_yushuensis">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Actinotignum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Actinotignum_timonense">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Varibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>57</val></magnitude>
       <node name="s__Varibaculum_prostatecancerukia">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Schaalia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>25653</val></magnitude>
       <node name="s__Schaalia_odontolytica">
        <magnitude><val>16859</val></magnitude>
       </node>
       <node name="s__Schaalia_sp._ZJ405">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Schaalia_sp._19OD2882">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Schaalia_cardiffensis">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Schaalia_meyeri">
        <magnitude><val>217</val></magnitude>
       </node>
       <node name="s__Schaalia_radingae">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Schaalia_sp._HMT-172">
        <magnitude><val>8232</val></magnitude>
       </node>
       <node name="s__Schaalia_sp._JY-X169">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Schaalia_turicensis">
        <magnitude><val>211</val></magnitude>
       </node>
      </node>
      <node name="g__Pauljensenia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>92</val></magnitude>
       <node name="s__Pauljensenia_hongkongensis">
        <magnitude><val>92</val></magnitude>
       </node>
      </node>
      <node name="g__Trueperella">
       <magnitude><val>87</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Trueperella_pyogenes">
        <magnitude><val>71</val></magnitude>
       </node>
       <node name="s__Trueperella_abortisuis">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Acidothermales">
     <magnitude><val>20</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Acidothermaceae">
      <magnitude><val>20</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Acidothermus">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Acidothermus_cellulolyticus">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Kitasatosporales">
     <magnitude><val>938</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Streptomycetaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>938</val></magnitude>
      <node name="g__Streptomyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>864</val></magnitude>
       <node name="s__Streptomyces_venezuelae">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._CB01881">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Streptomyces_seoulensis">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Streptomyces_olivoreticuli">
        <magnitude><val>89</val></magnitude>
       </node>
       <node name="s__Streptomyces_microflavus">
        <magnitude><val>167</val></magnitude>
       </node>
       <node name="s__Streptomyces_nigra">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Streptomyces_ferrugineus">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._INR7">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Streptomyces_formicae">
        <magnitude><val>32</val></magnitude>
       </node>
       <node name="s__Streptomyces_bathyalis">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._MA3_2.13">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._WMMC500">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Streptomyces_tsukubensis">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._CMB-StM0423">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Streptomyces_xiamenensis">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Streptomyces_collinus">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Streptomyces_paludis">
        <magnitude><val>82</val></magnitude>
       </node>
       <node name="s__Streptomyces_griseocarneus">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Streptomyces_sp._SCA4-21">
        <magnitude><val>66</val></magnitude>
       </node>
      </node>
      <node name="g__Streptacidiphilus">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Streptacidiphilus_sp._PB12-B1b">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Kitasatospora">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>61</val></magnitude>
       <node name="s__Kitasatospora_aureofaciens">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Kitasatospora_setae">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Jiangellales">
     <magnitude><val>13</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Jiangellaceae">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Jiangella">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Jiangella_alkaliphila">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Nitriliruptoria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>118</val></magnitude>
    <node name="o__Egibacterales">
     <magnitude><val>118</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Egibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>118</val></magnitude>
      <node name="g__Egibacter">
       <magnitude><val>118</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Egibacter_rhizosphaerae">
        <magnitude><val>118</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Lentisphaerota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>29</val></magnitude>
   <node name="c__Lentisphaeria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>29</val></magnitude>
    <node name="o__Lentisphaerales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>29</val></magnitude>
     <node name="f__Lentisphaeraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>29</val></magnitude>
      <node name="g__Lentisphaera">
       <magnitude><val>29</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lentisphaera_profundi">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Nitrospirota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>496</val></magnitude>
   <node name="c__Thermodesulfovibrionia">
    <magnitude><val>341</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Thermodesulfovibrionales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>341</val></magnitude>
     <node name="f__Dissulfurispiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>293</val></magnitude>
      <node name="g__Dissulfurispira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>293</val></magnitude>
       <node name="s__Dissulfurispira_thermophila">
        <magnitude><val>293</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Thermodesulfovibrionaceae">
      <magnitude><val>48</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Thermodesulfovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>48</val></magnitude>
       <node name="s__Thermodesulfovibrio_yellowstonii">
        <magnitude><val>48</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Nitrospiria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>155</val></magnitude>
    <node name="o__Nitrospirales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>155</val></magnitude>
     <node name="f__Nitrospiraceae">
      <magnitude><val>155</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Leptospirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>98</val></magnitude>
       <node name="s__Leptospirillum_ferrooxidans">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Leptospirillum_sp._Group_II_'CF-1'">
        <magnitude><val>47</val></magnitude>
       </node>
      </node>
      <node name="g__Nitrospira">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>57</val></magnitude>
       <node name="s__Candidatus_Nitrospira_inopinata">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Nitrospira_sp._KM1">
        <magnitude><val>42</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Bacteroidota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>3194292</val></magnitude>
   <node name="o__Candidatus_Sulfidibacteriales">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>20</val></magnitude>
    <node name="g__Candidatus_Sulfidibacterium">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>20</val></magnitude>
     <node name="s__Candidatus_Sulfidibacterium_hydrothermale">
      <magnitude><val>20</val></magnitude>
     </node>
    </node>
   </node>
   <node name="c__Chitinophagia">
    <magnitude><val>592</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Chitinophagales">
     <magnitude><val>592</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Chitinophagaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>592</val></magnitude>
      <node name="g__Sediminibacterium">
       <magnitude><val>28</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sediminibacterium_sp._TEGAF015">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Arachidicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>175</val></magnitude>
       <node name="s__Arachidicoccus_soli">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Arachidicoccus_ginsenosidivorans">
        <magnitude><val>85</val></magnitude>
       </node>
       <node name="s__Arachidicoccus_sp._BS20">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Arachidicoccus_terrestris">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Paraflavitalea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>18</val></magnitude>
       <node name="s__Paraflavitalea_soli">
        <magnitude><val>18</val></magnitude>
       </node>
      </node>
      <node name="g__Lacibacter">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lacibacter_sediminis">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Niabella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Niabella_ginsenosidivorans">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Niabella_soli">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Flavisolibacter">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Flavisolibacter_tropicus">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Chitinophaga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>259</val></magnitude>
       <node name="s__Chitinophaga_horti">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Chitinophaga_sp._XS-30">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Chitinophaga_agri">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Chitinophaga_filiformis">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Chitinophaga_caeni">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Chitinophaga_sp._HK235">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Chitinophaga_pinensis">
        <magnitude><val>136</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudocnuella">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pseudocnuella_soli">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Sphingobacteriia">
    <magnitude><val>1160</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Sphingobacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1160</val></magnitude>
     <node name="f__Sphingobacteriaceae">
      <magnitude><val>1141</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pedobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>323</val></magnitude>
       <node name="s__Pedobacter_sp.">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Pedobacter_sp._HDW13">
        <magnitude><val>38</val></magnitude>
       </node>
       <node name="s__Pedobacter_sp._D749">
        <magnitude><val>43</val></magnitude>
       </node>
       <node name="s__Pedobacter_schmidteae">
        <magnitude><val>42</val></magnitude>
       </node>
       <node name="s__Pedobacter_riviphilus">
        <magnitude><val>34</val></magnitude>
       </node>
       <node name="s__Pedobacter_ginsengisoli">
        <magnitude><val>129</val></magnitude>
       </node>
      </node>
      <node name="g__Anseongella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Anseongella_ginsenosidimutans">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Sphingobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>394</val></magnitude>
       <node name="s__Sphingobacterium_sp._WM">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._KACC_22765">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_daejeonense">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._LZ7M1">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._PCS056">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._SYP-B4668">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_hotanense">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_faecium">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_lactis">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._ML3W">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_spiritivorum">
        <magnitude><val>101</val></magnitude>
       </node>
       <node name="s__Sphingobacterium_sp._DR205">
        <magnitude><val>27</val></magnitude>
       </node>
      </node>
      <node name="g__Olivibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Olivibacter_sp._SDN3">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Mucilaginibacter">
       <magnitude><val>360</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mucilaginibacter_sp._KACC_22773">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Mucilaginibacter_xinganensis">
        <magnitude><val>68</val></magnitude>
       </node>
       <node name="s__Mucilaginibacter_sp._KACC_22063">
        <magnitude><val>111</val></magnitude>
       </node>
       <node name="s__Mucilaginibacter_mali">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Mucilaginibacter_ginkgonis">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Mucilaginibacter_rubeus">
        <magnitude><val>95</val></magnitude>
       </node>
      </node>
      <node name="g__Solitalea">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>44</val></magnitude>
       <node name="s__Solitalea_lacus">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Aurantibacillaceae">
      <magnitude><val>19</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Aurantibacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Aurantibacillus_circumpalustris">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Saprospiria">
    <magnitude><val>60</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Saprospirales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>60</val></magnitude>
     <node name="f__Saprospiraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>60</val></magnitude>
      <node name="g__Saprospira">
       <magnitude><val>44</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Saprospira_sp._CCB-QB6">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
      <node name="g__Aureispira">
       <magnitude><val>16</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aureispira_sp._EL160426">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Cytophagia">
    <magnitude><val>1492</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Cytophagales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>1492</val></magnitude>
     <node name="f__Cytophagaceae">
      <magnitude><val>234</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Spirosoma">
       <magnitude><val>202</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Spirosoma_sp._KCTC_42546">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Spirosoma_endbachense">
        <magnitude><val>151</val></magnitude>
       </node>
       <node name="s__Spirosoma_sp._KUDC1026">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Aquirufa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Aquirufa_nivalisilvae">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Tellurirhabdus">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tellurirhabdus_rosea">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Catalimonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>39</val></magnitude>
      <node name="g__Catalinimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>39</val></magnitude>
       <node name="s__Catalinimonas_niigatensis">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Cyclobacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>186</val></magnitude>
      <node name="g__Mongoliitalea">
       <magnitude><val>67</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Mongoliitalea_daihaiensis">
        <magnitude><val>67</val></magnitude>
       </node>
      </node>
      <node name="g__Algoriphagus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>86</val></magnitude>
       <node name="s__Algoriphagus_sp._Y33">
        <magnitude><val>40</val></magnitude>
       </node>
       <node name="s__Algoriphagus_sanaruensis">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Aquiflexum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>12</val></magnitude>
       <node name="s__Aquiflexum_balticum">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Echinicola">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Echinicola_soli">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Fulvivirgaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>72</val></magnitude>
      <node name="g__Fulvivirga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>38</val></magnitude>
       <node name="s__Fulvivirga_ligni">
        <magnitude><val>38</val></magnitude>
       </node>
      </node>
      <node name="g__Chryseolinea">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Chryseolinea_soli">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Spirosomataceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>275</val></magnitude>
      <node name="g__Emticicia">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Emticicia_oligotrophica">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Runella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Runella_sp._SP2">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Dyadobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>120</val></magnitude>
       <node name="s__Dyadobacter_fermentans">
        <magnitude><val>59</val></magnitude>
       </node>
       <node name="s__Dyadobacter_sp._NIV53">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Dyadobacter_sandarakinus">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Dyadobacter_pollutisoli">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
      <node name="g__Leadbetterella">
       <magnitude><val>32</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leadbetterella_byssophila">
        <magnitude><val>32</val></magnitude>
       </node>
      </node>
      <node name="g__Marinilongibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>63</val></magnitude>
       <node name="s__Marinilongibacter_aquaticus">
        <magnitude><val>63</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Marivirgaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>28</val></magnitude>
      <node name="g__Marivirga">
       <magnitude><val>28</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marivirga_tractuosa">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Mangrovivirgaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>15</val></magnitude>
      <node name="g__Mangrovivirga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>15</val></magnitude>
       <node name="s__Mangrovivirga_cuniculi">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Hymenobacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>488</val></magnitude>
      <node name="g__Pontibacter">
       <magnitude><val>75</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pontibacter_actiniarum">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Pontibacter_sp._SGAir0037">
        <magnitude><val>51</val></magnitude>
       </node>
      </node>
      <node name="g__Hymenobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>347</val></magnitude>
       <node name="s__Hymenobacter_aerilatus">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Hymenobacter_volaticus">
        <magnitude><val>326</val></magnitude>
       </node>
      </node>
      <node name="g__Adhaeribacter">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Adhaeribacter_radiodurans">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Nibribacter">
       <magnitude><val>52</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nibribacter_ruber">
        <magnitude><val>52</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Reichenbachiellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>34</val></magnitude>
      <node name="g__Reichenbachiella">
       <magnitude><val>34</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Reichenbachiella_sp._Wsw4-B4">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Flammeovirgaceae">
      <magnitude><val>121</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Imperialibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Imperialibacter_roseus">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
      <node name="g__Flammeovirga">
       <magnitude><val>104</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Flammeovirga_sp._MY04">
        <magnitude><val>104</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Bacteroidia">
    <magnitude><val>3183944</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Marinilabiliales">
     <magnitude><val>579</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Marinifilaceae">
      <magnitude><val>50</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Labilibaculum">
       <magnitude><val>50</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Labilibaculum_antarcticum">
        <magnitude><val>50</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Marinilabiliaceae">
      <magnitude><val>21</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Carboxylicivirga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__uncultured_Carboxylicivirga_sp.">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Prolixibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>508</val></magnitude>
      <node name="g__Aquipluma">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aquipluma_nitroreducens">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Maribellus">
       <magnitude><val>33</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Maribellus_comscasis">
        <magnitude><val>33</val></magnitude>
       </node>
      </node>
      <node name="g__Draconibacterium">
       <magnitude><val>464</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Draconibacterium_orientale">
        <magnitude><val>46</val></magnitude>
       </node>
       <node name="s__uncultured_Draconibacterium_sp.">
        <magnitude><val>418</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Bacteroidales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>3183365</val></magnitude>
     <node name="f__Tannerellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>249096</val></magnitude>
      <node name="g__Tannerella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>187</val></magnitude>
       <node name="s__Tannerella_serpentiformis">
        <magnitude><val>187</val></magnitude>
       </node>
      </node>
      <node name="g__Parabacteroides">
       <magnitude><val>248909</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Parabacteroides_distasonis">
        <magnitude><val>91582</val></magnitude>
       </node>
       <node name="s__Parabacteroides_chongii">
        <magnitude><val>348</val></magnitude>
       </node>
       <node name="s__Parabacteroides_faecis">
        <magnitude><val>298</val></magnitude>
       </node>
       <node name="s__Parabacteroides_johnsonii">
        <magnitude><val>395</val></magnitude>
       </node>
       <node name="s__Parabacteroides_merdae">
        <magnitude><val>56101</val></magnitude>
       </node>
       <node name="s__Parabacteroides_sp._CT06">
        <magnitude><val>99459</val></magnitude>
       </node>
       <node name="s__Parabacteroides_goldsteinii">
        <magnitude><val>726</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Dysgonomonadaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>34</val></magnitude>
      <node name="g__Proteiniphilum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20</val></magnitude>
       <node name="s__Proteiniphilum_propionicum">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Petrimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Petrimonas_mucosa">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Bacteroidaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>2607822</val></magnitude>
      <node name="g__Phocaeicola">
       <magnitude><val>1130142</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Phocaeicola_vulgatus">
        <magnitude><val>709791</val></magnitude>
       </node>
       <node name="s__Phocaeicola_salanitronis">
        <magnitude><val>1537</val></magnitude>
       </node>
       <node name="s__Phocaeicola_coprophilus">
        <magnitude><val>471</val></magnitude>
       </node>
       <node name="s__Phocaeicola_dorei">
        <magnitude><val>418343</val></magnitude>
       </node>
      </node>
      <node name="g__Bacteroides">
       <magnitude><val>1477680</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Bacteroides_sp._ZJ-18">
        <magnitude><val>548</val></magnitude>
       </node>
       <node name="s__Bacteroides_zhangwenhongii">
        <magnitude><val>819</val></magnitude>
       </node>
       <node name="s__Bacteroides_caecimuris">
        <magnitude><val>2473</val></magnitude>
       </node>
       <node name="s__Bacteroides_coprosuis">
        <magnitude><val>24</val></magnitude>
       </node>
       <node name="s__Bacteroides_thetaiotaomicron">
        <magnitude><val>223145</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._M10">
        <magnitude><val>2748</val></magnitude>
       </node>
       <node name="s__Bacteroides_humanifaecis">
        <magnitude><val>1780</val></magnitude>
       </node>
       <node name="s__Bacteroides_caccae">
        <magnitude><val>3121</val></magnitude>
       </node>
       <node name="s__Bacteroides_cellulosilyticus">
        <magnitude><val>1234</val></magnitude>
       </node>
       <node name="s__Bacteroides_xylanisolvens">
        <magnitude><val>22633</val></magnitude>
       </node>
       <node name="s__Bacteroides_luhongzhouii">
        <magnitude><val>1740</val></magnitude>
       </node>
       <node name="s__Bacteroides_uniformis">
        <magnitude><val>310414</val></magnitude>
       </node>
       <node name="s__Bacteroides_helcogenes">
        <magnitude><val>194</val></magnitude>
       </node>
       <node name="s__Bacteroides_salyersiae">
        <magnitude><val>3883</val></magnitude>
       </node>
       <node name="s__Bacteroides_faecis">
        <magnitude><val>21052</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._D2">
        <magnitude><val>4447</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._A1C1">
        <magnitude><val>6021</val></magnitude>
       </node>
       <node name="s__Bacteroides_faecium">
        <magnitude><val>364</val></magnitude>
       </node>
       <node name="s__Bacteroides_nordii">
        <magnitude><val>239</val></magnitude>
       </node>
       <node name="s__Bacteroides_heparinolyticus">
        <magnitude><val>166</val></magnitude>
       </node>
       <node name="s__Bacteroides_fragilis">
        <magnitude><val>16396</val></magnitude>
       </node>
       <node name="s__Bacteroides_graminisolvens">
        <magnitude><val>56</val></magnitude>
       </node>
       <node name="s__Bacteroides_ovatus">
        <magnitude><val>181581</val></magnitude>
       </node>
       <node name="s__Bacteroides_stercoris">
        <magnitude><val>2068</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._PHL_2737">
        <magnitude><val>14920</val></magnitude>
       </node>
       <node name="s__Bacteroides_zoogleoformans">
        <magnitude><val>136</val></magnitude>
       </node>
       <node name="s__Bacteroides_intestinalis">
        <magnitude><val>745</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._BFG-257">
        <magnitude><val>2605</val></magnitude>
       </node>
       <node name="s__Bacteroides_eggerthii">
        <magnitude><val>622213</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._CACC_737">
        <magnitude><val>14489</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._DH3716P">
        <magnitude><val>4628</val></magnitude>
       </node>
       <node name="s__Bacteroides_sp._HF-162">
        <magnitude><val>10798</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Rikenellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>297256</val></magnitude>
      <node name="g__Alistipes">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>297256</val></magnitude>
       <node name="s__Alistipes_finegoldii">
        <magnitude><val>277750</val></magnitude>
       </node>
       <node name="s__Alistipes_communis">
        <magnitude><val>1047</val></magnitude>
       </node>
       <node name="s__uncultured_Alistipes_sp.">
        <magnitude><val>80</val></magnitude>
       </node>
       <node name="s__Alistipes_onderdonkii">
        <magnitude><val>5912</val></magnitude>
       </node>
       <node name="s__Alistipes_shahii">
        <magnitude><val>5012</val></magnitude>
       </node>
       <node name="s__Alistipes_dispar">
        <magnitude><val>139</val></magnitude>
       </node>
       <node name="s__Alistipes_megaguti">
        <magnitude><val>186</val></magnitude>
       </node>
       <node name="s__Alistipes_senegalensis">
        <magnitude><val>7029</val></magnitude>
       </node>
       <node name="s__Alistipes_indistinctus">
        <magnitude><val>62</val></magnitude>
       </node>
       <node name="s__Alistipes_ihumii">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Alistipes_sp._dk3624">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Prevotellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>4942</val></magnitude>
      <node name="g__Prevotella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2791</val></magnitude>
       <node name="s__Prevotella_herbatica">
        <magnitude><val>282</val></magnitude>
       </node>
       <node name="s__Prevotella_sp._E9-3">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Prevotella_communis">
        <magnitude><val>74</val></magnitude>
       </node>
       <node name="s__Prevotella_fusca">
        <magnitude><val>640</val></magnitude>
       </node>
       <node name="s__Prevotella_denticola">
        <magnitude><val>51</val></magnitude>
       </node>
       <node name="s__Prevotella_sp._oral_taxon_475">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Prevotella_ruminicola">
        <magnitude><val>176</val></magnitude>
       </node>
       <node name="s__Prevotella_sp._E2-28">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Prevotella_melaninogenica">
        <magnitude><val>744</val></magnitude>
       </node>
       <node name="s__Prevotella_nigrescens">
        <magnitude><val>193</val></magnitude>
       </node>
       <node name="s__Prevotella_scopos">
        <magnitude><val>100</val></magnitude>
       </node>
       <node name="s__Prevotella_bivia">
        <magnitude><val>15</val></magnitude>
       </node>
       <node name="s__Prevotella_intermedia">
        <magnitude><val>126</val></magnitude>
       </node>
       <node name="s__Prevotella_jejuni">
        <magnitude><val>257</val></magnitude>
       </node>
       <node name="s__Prevotella_corporis">
        <magnitude><val>59</val></magnitude>
       </node>
      </node>
      <node name="g__Pseudoprevotella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>77</val></magnitude>
       <node name="s__Pseudoprevotella_muciniphila">
        <magnitude><val>77</val></magnitude>
       </node>
      </node>
      <node name="g__Segatella">
       <magnitude><val>585</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Segatella_oris">
        <magnitude><val>48</val></magnitude>
       </node>
       <node name="s__Segatella_hominis">
        <magnitude><val>161</val></magnitude>
       </node>
       <node name="s__Segatella_copri">
        <magnitude><val>376</val></magnitude>
       </node>
      </node>
      <node name="g__Paraprevotella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>285</val></magnitude>
       <node name="s__Paraprevotella_clara">
        <magnitude><val>96</val></magnitude>
       </node>
       <node name="s__Paraprevotella_xylaniphila">
        <magnitude><val>189</val></magnitude>
       </node>
      </node>
      <node name="g__Hoylesella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1204</val></magnitude>
       <node name="s__Hoylesella_buccalis">
        <magnitude><val>1132</val></magnitude>
       </node>
       <node name="s__Hoylesella_enoeca">
        <magnitude><val>72</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Paludibacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>17</val></magnitude>
      <node name="g__Paludibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Paludibacter_propionicigenes">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Barnesiellaceae">
      <magnitude><val>1610</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Coprobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>310</val></magnitude>
       <node name="s__Coprobacter_fastidiosus">
        <magnitude><val>149</val></magnitude>
       </node>
       <node name="s__Coprobacter_secundus">
        <magnitude><val>161</val></magnitude>
       </node>
      </node>
      <node name="g__Barnesiella">
       <magnitude><val>1300</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Barnesiella_viscericola">
        <magnitude><val>1300</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Salinivirgaceae">
      <magnitude><val>62</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Salinivirga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>62</val></magnitude>
       <node name="s__Salinivirga_cyanobacteriivorans">
        <magnitude><val>62</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Porphyromonadaceae">
      <magnitude><val>59</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Porphyromonas">
       <magnitude><val>59</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Porphyromonas_gingivalis">
        <magnitude><val>20</val></magnitude>
       </node>
       <node name="s__Porphyromonas_somerae">
        <magnitude><val>10</val></magnitude>
       </node>
       <node name="s__Porphyromonas_endodontalis">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Porphyromonas_asaccharolytica">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Muribaculaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>535</val></magnitude>
      <node name="g__Paramuribaculum">
       <magnitude><val>299</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Paramuribaculum_intestinale">
        <magnitude><val>299</val></magnitude>
       </node>
      </node>
      <node name="g__Sodaliphilus">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sodaliphilus_pleomorphus">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Muribaculum">
       <magnitude><val>93</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Muribaculum_intestinale">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Muribaculum_gordoncarteri">
        <magnitude><val>63</val></magnitude>
       </node>
      </node>
      <node name="g__Duncaniella">
       <magnitude><val>130</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Duncaniella_dubosii">
        <magnitude><val>130</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Odoribacteraceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>21932</val></magnitude>
      <node name="g__Odoribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>20117</val></magnitude>
       <node name="s__Odoribacter_splanchnicus">
        <magnitude><val>20117</val></magnitude>
       </node>
      </node>
      <node name="g__Butyricimonas">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1815</val></magnitude>
       <node name="s__Butyricimonas_faecihominis">
        <magnitude><val>528</val></magnitude>
       </node>
       <node name="s__Butyricimonas_faecalis">
        <magnitude><val>161</val></magnitude>
       </node>
       <node name="s__Butyricimonas_virosa">
        <magnitude><val>954</val></magnitude>
       </node>
       <node name="s__Butyricimonas_paravirosa">
        <magnitude><val>172</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Flavobacteriia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>7024</val></magnitude>
    <node name="o__Flavobacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>7024</val></magnitude>
     <node name="f__Weeksellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>3068</val></magnitude>
      <node name="g__Empedobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>28</val></magnitude>
       <node name="s__Empedobacter_stercoris">
        <magnitude><val>28</val></magnitude>
       </node>
      </node>
      <node name="g__Elizabethkingia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>252</val></magnitude>
       <node name="s__Elizabethkingia_ursingii">
        <magnitude><val>203</val></magnitude>
       </node>
       <node name="s__Elizabethkingia_meningoseptica">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Elizabethkingia_miricola">
        <magnitude><val>24</val></magnitude>
       </node>
      </node>
      <node name="g__Riemerella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>200</val></magnitude>
       <node name="s__Riemerella_anatipestifer">
        <magnitude><val>200</val></magnitude>
       </node>
      </node>
      <node name="g__Marnyiella">
       <magnitude><val>182</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marnyiella_aurantia">
        <magnitude><val>182</val></magnitude>
       </node>
      </node>
      <node name="g__Chryseobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>2277</val></magnitude>
       <node name="s__Chryseobacterium_capnotolerans">
        <magnitude><val>92</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_camelliae">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_gallinarum">
        <magnitude><val>478</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_indoltheticum">
        <magnitude><val>101</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_aureum">
        <magnitude><val>92</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_shandongense">
        <magnitude><val>165</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_faecale">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._MMS21-Ot14">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_arthrosphaerae">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._G0201">
        <magnitude><val>66</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_taklimakanense">
        <magnitude><val>306</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._IHB_B_17019">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_nepalense">
        <magnitude><val>259</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_oranimense">
        <magnitude><val>113</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_oryzae">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp.">
        <magnitude><val>175</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._T16E-39">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._POL2">
        <magnitude><val>116</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._LJ668">
        <magnitude><val>122</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_indologenes">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Chryseobacterium_sp._Y16C">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Bergeyella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>34</val></magnitude>
       <node name="s__Bergeyella_cardium">
        <magnitude><val>34</val></magnitude>
       </node>
      </node>
      <node name="g__Kaistella">
       <magnitude><val>95</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kaistella_daneshvariae">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Kaistella_antarctica">
        <magnitude><val>83</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Blattabacteriaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>244</val></magnitude>
      <node name="g__Blattabacterium">
       <magnitude><val>244</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Blattabacterium_cuenoti">
        <magnitude><val>244</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Flavobacteriaceae">
      <magnitude><val>3695</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cellulophaga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>80</val></magnitude>
       <node name="s__Cellulophaga_omnivescoria">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Cellulophaga_sp._L1A9">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Cellulophaga_lytica">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Cellulophaga_sp._HaHaR_3_176">
        <magnitude><val>16</val></magnitude>
       </node>
      </node>
      <node name="g__Winogradskyella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>44</val></magnitude>
       <node name="s__Winogradskyella_sp._PC-19">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
      <node name="g__Lacinutrix">
       <magnitude><val>20</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lacinutrix_sp._Bg11-31">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Nonlabens">
       <magnitude><val>105</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Nonlabens_ponticola">
        <magnitude><val>12</val></magnitude>
       </node>
       <node name="s__Nonlabens_ulvanivorans">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Nonlabens_dokdonensis">
        <magnitude><val>57</val></magnitude>
       </node>
      </node>
      <node name="g__Tamlana">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tamlana_carrageenivorans">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Arenibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Arenibacter_algicola">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Urechidicola">
       <magnitude><val>26</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Urechidicola_croceus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Polaribacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>156</val></magnitude>
       <node name="s__Polaribacter_cellanae">
        <magnitude><val>37</val></magnitude>
       </node>
       <node name="s__Polaribacter_sp._R2A056_3_33">
        <magnitude><val>99</val></magnitude>
       </node>
       <node name="s__Polaribacter_sp._MED152">
        <magnitude><val>20</val></magnitude>
       </node>
      </node>
      <node name="g__Formosa">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>39</val></magnitude>
       <node name="s__Formosa_sp._L2A11">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Formosa_sediminum">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
      <node name="g__Flaviramulus">
       <magnitude><val>48</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Flaviramulus_sp._BrNp1-15">
        <magnitude><val>48</val></magnitude>
       </node>
      </node>
      <node name="g__Flavobacterium">
       <magnitude><val>1841</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Flavobacterium_sp._F-70">
        <magnitude><val>61</val></magnitude>
       </node>
       <node name="s__Flavobacterium_oreochromis">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Flavobacterium_nitrogenifigens">
        <magnitude><val>57</val></magnitude>
       </node>
       <node name="s__uncultured_Flavobacterium_sp.">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._N502540">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._YJ01">
        <magnitude><val>176</val></magnitude>
       </node>
       <node name="s__Flavobacterium_cerinum">
        <magnitude><val>67</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._N1736">
        <magnitude><val>155</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._N2820">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._B183">
        <magnitude><val>23</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._N3904">
        <magnitude><val>13</val></magnitude>
       </node>
       <node name="s__Flavobacterium_okayamense">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._ZE23DGlu08">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Flavobacterium_inviolabile">
        <magnitude><val>33</val></magnitude>
       </node>
       <node name="s__Flavobacterium_channae">
        <magnitude><val>45</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sediminis">
        <magnitude><val>95</val></magnitude>
       </node>
       <node name="s__Flavobacterium_pectinovorum">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._CECT_9288">
        <magnitude><val>229</val></magnitude>
       </node>
       <node name="s__Flavobacterium_gelatinilyticum">
        <magnitude><val>62</val></magnitude>
       </node>
       <node name="s__Flavobacterium_nackdongense">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._CJ74">
        <magnitude><val>103</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._CJ75">
        <magnitude><val>52</val></magnitude>
       </node>
       <node name="s__Flavobacterium_bizetiae">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Flavobacterium_gyeonganense">
        <magnitude><val>18</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._F-29">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Flavobacterium_johnsoniae">
        <magnitude><val>60</val></magnitude>
       </node>
       <node name="s__Flavobacterium_sp._GSB-24">
        <magnitude><val>270</val></magnitude>
       </node>
       <node name="s__Flavobacterium_davisii">
        <magnitude><val>77</val></magnitude>
       </node>
      </node>
      <node name="g__Maribacter">
       <magnitude><val>40</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Maribacter_sp._Hal144">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Maribacter_litopenaei">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
      <node name="g__Aureibaculum">
       <magnitude><val>13</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aureibaculum_algae">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Seonamhaeicola">
       <magnitude><val>72</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Seonamhaeicola_sp._ML3">
        <magnitude><val>72</val></magnitude>
       </node>
      </node>
      <node name="g__Psychroflexus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Psychroflexus_torquis">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
      <node name="g__Sinomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>46</val></magnitude>
       <node name="s__Sinomicrobium_kalidii">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Kordia">
       <magnitude><val>15</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Kordia_sp._SMS9">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Croceibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>45</val></magnitude>
       <node name="s__Croceibacter_atlanticus">
        <magnitude><val>45</val></magnitude>
       </node>
      </node>
      <node name="g__Myroides">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Myroides_odoratus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Christiangramia">
       <magnitude><val>120</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Christiangramia_flava">
        <magnitude><val>19</val></magnitude>
       </node>
       <node name="s__Christiangramia_forsetii">
        <magnitude><val>90</val></magnitude>
       </node>
       <node name="s__Christiangramia_salexigens">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Dokdonia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>308</val></magnitude>
       <node name="s__Dokdonia_sp._PRO95">
        <magnitude><val>308</val></magnitude>
       </node>
      </node>
      <node name="g__Salegentibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__Salegentibacter_sp._T436">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
      <node name="g__Aquimarina">
       <magnitude><val>65</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Aquimarina_sp._ERC-38">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Aquimarina_sp._BL5">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Antarcticibacterium">
       <magnitude><val>134</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Antarcticibacterium_arcticum">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Antarcticibacterium_sp._1MA-6-2">
        <magnitude><val>105</val></magnitude>
       </node>
      </node>
      <node name="g__Allomuricauda">
       <magnitude><val>45</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Allomuricauda_aurantiaca">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Allomuricauda_lutaonensis">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
      <node name="g__Tenacibaculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Tenacibaculum_maritimum">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Gillisia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Gillisia_sp._Hel1_33_143">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Lutibacter">
       <magnitude><val>46</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Lutibacter_sp._A80">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
      <node name="g__Capnocytophaga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>224</val></magnitude>
       <node name="s__Capnocytophaga_stomatis">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Capnocytophaga_leadbetteri">
        <magnitude><val>84</val></magnitude>
       </node>
       <node name="s__Capnocytophaga_sputigena">
        <magnitude><val>25</val></magnitude>
       </node>
       <node name="s__Capnocytophaga_sp._oral_taxon_878">
        <magnitude><val>99</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Crocinitomicaceae">
      <magnitude><val>17</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Paracrocinitomix">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>17</val></magnitude>
       <node name="s__Paracrocinitomix_mangrovi">
        <magnitude><val>17</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Myxococcota">
   <magnitude><val>327</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="o__Nannocystales">
    <magnitude><val>14</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="f__Nannocystaceae">
     <magnitude><val>14</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Nannocystis">
      <magnitude><val>14</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Nannocystis_poenicansa">
       <magnitude><val>14</val></magnitude>
      </node>
     </node>
    </node>
   </node>
   <node name="o__Haliangiales">
    <magnitude><val>17</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="f__Kofleriaceae">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>17</val></magnitude>
     <node name="g__Haliangium">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>17</val></magnitude>
      <node name="s__Haliangium_ochraceum">
       <magnitude><val>17</val></magnitude>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Myxococcia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>184</val></magnitude>
    <node name="o__Myxococcales">
     <magnitude><val>184</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Archangiaceae">
      <magnitude><val>48</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cystobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>22</val></magnitude>
       <node name="s__Cystobacter_fuscus">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
      <node name="g__Melittangium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Melittangium_boletus">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Myxococcaceae">
      <magnitude><val>54</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Myxococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>40</val></magnitude>
       <node name="s__Myxococcus_xanthus">
        <magnitude><val>40</val></magnitude>
       </node>
      </node>
      <node name="g__Pyxidicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Pyxidicoccus_parkwaysis">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Anaeromyxobacteraceae">
      <magnitude><val>82</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Anaeromyxobacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>82</val></magnitude>
       <node name="s__Anaeromyxobacter_sp._Fw109-5">
        <magnitude><val>36</val></magnitude>
       </node>
       <node name="s__Anaeromyxobacter_oryzae">
        <magnitude><val>46</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="o__Polyangiales">
    <magnitude><val>112</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="f__Sandaracinaceae">
     <magnitude><val>13</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Sandaracinus">
      <magnitude><val>13</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Sandaracinus_amylolyticus">
       <magnitude><val>13</val></magnitude>
      </node>
     </node>
    </node>
    <node name="f__Polyangiaceae">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>72</val></magnitude>
     <node name="g__Sorangium">
      <magnitude><val>72</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="s__Sorangium_cellulosum">
       <magnitude><val>72</val></magnitude>
      </node>
     </node>
    </node>
    <node name="f__Labilitrichaceae">
     <magnitude><val>27</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="g__Labilithrix">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>27</val></magnitude>
      <node name="s__Labilithrix_luteola">
       <magnitude><val>27</val></magnitude>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Deferribacterota">
   <magnitude><val>449</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Deferribacteres">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>449</val></magnitude>
    <node name="o__Deferribacterales">
     <magnitude><val>449</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Mucispirillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>148</val></magnitude>
      <node name="g__Mucispirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>148</val></magnitude>
       <node name="s__Mucispirillum_schaedleri">
        <magnitude><val>148</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Calditerrivibrionaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>12</val></magnitude>
      <node name="g__Calditerrivibrio">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Calditerrivibrio_nitroreducens">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Geovibrionaceae">
      <magnitude><val>289</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Geovibrio">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__Geovibrio_thiophilus">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
      <node name="g__Denitrovibrio">
       <magnitude><val>253</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Denitrovibrio_acetiphilus">
        <magnitude><val>253</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Fusobacteriota">
   <magnitude><val>2700</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Fusobacteriia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>2700</val></magnitude>
    <node name="o__Fusobacteriales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>2700</val></magnitude>
     <node name="f__Leptotrichiaceae">
      <magnitude><val>559</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pseudoleptotrichia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Pseudoleptotrichia_goodfellowii">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
      <node name="g__Sebaldella">
       <magnitude><val>101</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Sebaldella_termitidis">
        <magnitude><val>101</val></magnitude>
       </node>
      </node>
      <node name="g__Streptobacillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>43</val></magnitude>
       <node name="s__Streptobacillus_moniliformis">
        <magnitude><val>43</val></magnitude>
       </node>
      </node>
      <node name="g__Leptotrichia">
       <magnitude><val>404</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Leptotrichia_sp._oral_taxon_221">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Leptotrichia_shahii">
        <magnitude><val>22</val></magnitude>
       </node>
       <node name="s__Leptotrichia_sp._oral_taxon_847">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Leptotrichia_buccalis">
        <magnitude><val>103</val></magnitude>
       </node>
       <node name="s__Leptotrichia_wadei">
        <magnitude><val>215</val></magnitude>
       </node>
       <node name="s__Leptotrichia_sp._oral_taxon_212">
        <magnitude><val>22</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Fusobacteriaceae">
      <magnitude><val>2054</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cetobacterium">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cetobacterium_somerae">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Ilyobacter">
       <magnitude><val>142</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Ilyobacter_sp.">
        <magnitude><val>54</val></magnitude>
       </node>
       <node name="s__Ilyobacter_polytropus">
        <magnitude><val>88</val></magnitude>
       </node>
      </node>
      <node name="g__Fusobacterium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>1898</val></magnitude>
       <node name="s__Fusobacterium_varium">
        <magnitude><val>39</val></magnitude>
       </node>
       <node name="s__Fusobacterium_nucleatum">
        <magnitude><val>134</val></magnitude>
       </node>
       <node name="s__Fusobacterium_hominis">
        <magnitude><val>210</val></magnitude>
       </node>
       <node name="s__Fusobacterium_gonidiaformans">
        <magnitude><val>41</val></magnitude>
       </node>
       <node name="s__Fusobacterium_necrophorum">
        <magnitude><val>91</val></magnitude>
       </node>
       <node name="s__Fusobacterium_pseudoperiodonticum">
        <magnitude><val>29</val></magnitude>
       </node>
       <node name="s__Fusobacterium_ulcerans">
        <magnitude><val>239</val></magnitude>
       </node>
       <node name="s__Fusobacterium_mortiferum">
        <magnitude><val>28</val></magnitude>
       </node>
       <node name="s__Fusobacterium_gastrosuis">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Fusobacterium_vincentii">
        <magnitude><val>1060</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Haliovirgaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>87</val></magnitude>
      <node name="g__Haliovirga">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>87</val></magnitude>
       <node name="s__Haliovirga_abyssi">
        <magnitude><val>87</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
 </node>
 <node name="k__Eukaryota">
  <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
  <magnitude><val>11322</val></magnitude>
  <node name="p__Ascomycota">
   <magnitude><val>10925</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Dothideomycetes">
    <magnitude><val>11</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Mycosphaerellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>11</val></magnitude>
     <node name="f__Mycosphaerellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>11</val></magnitude>
      <node name="g__Cercospora">
       <magnitude><val>11</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cercospora_beticola">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Eurotiomycetes">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>81</val></magnitude>
    <node name="o__Eurotiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>81</val></magnitude>
     <node name="f__Aspergillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>52</val></magnitude>
      <node name="g__Aspergillus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>52</val></magnitude>
       <node name="s__Aspergillus_luchuensis">
        <magnitude><val>11</val></magnitude>
       </node>
       <node name="s__Aspergillus_puulaauensis">
        <magnitude><val>27</val></magnitude>
       </node>
       <node name="s__Aspergillus_fumigatus">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Trichocomaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>29</val></magnitude>
      <node name="g__Talaromyces">
       <magnitude><val>29</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Talaromyces_marneffei">
        <magnitude><val>29</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Sordariomycetes">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>466</val></magnitude>
    <node name="o__Hypocreales">
     <magnitude><val>273</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Hypocreaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>35</val></magnitude>
      <node name="g__Trichoderma">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>35</val></magnitude>
       <node name="s__Trichoderma_breve">
        <magnitude><val>35</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Nectriaceae">
      <magnitude><val>238</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Fusarium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>238</val></magnitude>
       <node name="s__Fusarium_graminearum">
        <magnitude><val>31</val></magnitude>
       </node>
       <node name="s__Fusarium_fujikuroi">
        <magnitude><val>81</val></magnitude>
       </node>
       <node name="s__Fusarium_verticillioides">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Fusarium_keratoplasticum">
        <magnitude><val>100</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Magnaporthales">
     <magnitude><val>100</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Pyriculariaceae">
      <magnitude><val>100</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Pyricularia">
       <magnitude><val>100</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Pyricularia_pennisetigena">
        <magnitude><val>14</val></magnitude>
       </node>
       <node name="s__Pyricularia_grisea">
        <magnitude><val>86</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Glomerellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>44</val></magnitude>
     <node name="f__Glomerellaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>44</val></magnitude>
      <node name="g__Colletotrichum">
       <magnitude><val>44</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Colletotrichum_lupini">
        <magnitude><val>44</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Sordariales">
     <magnitude><val>49</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Chaetomiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>49</val></magnitude>
      <node name="g__Thermothielavioides">
       <magnitude><val>12</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermothielavioides_terrestris">
        <magnitude><val>12</val></magnitude>
       </node>
      </node>
      <node name="g__Thermothelomyces">
       <magnitude><val>37</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Thermothelomyces_thermophilus">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Saccharomycetes">
    <magnitude><val>10356</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Saccharomycetales">
     <magnitude><val>10356</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Saccharomycetaceae">
      <magnitude><val>10256</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Kluyveromyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>26</val></magnitude>
       <node name="s__Kluyveromyces_lactis">
        <magnitude><val>26</val></magnitude>
       </node>
      </node>
      <node name="g__Torulaspora">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>70</val></magnitude>
       <node name="s__Torulaspora_delbrueckii">
        <magnitude><val>70</val></magnitude>
       </node>
      </node>
      <node name="g__Tetrapisispora">
       <magnitude><val>108</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Tetrapisispora_blattae">
        <magnitude><val>83</val></magnitude>
       </node>
       <node name="s__Tetrapisispora_phaffii">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Saccharomyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10052</val></magnitude>
       <node name="s__Saccharomyces_cerevisiae">
        <magnitude><val>9996</val></magnitude>
       </node>
       <node name="s__Saccharomyces_mikatae">
        <magnitude><val>17</val></magnitude>
       </node>
       <node name="s__Saccharomyces_paradoxus">
        <magnitude><val>39</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Debaryomycetaceae">
      <magnitude><val>10</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Candida">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>10</val></magnitude>
       <node name="s__Candida_dubliniensis">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Pichiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>21</val></magnitude>
      <node name="g__Pichia">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>21</val></magnitude>
       <node name="s__Pichia_kudriavzevii">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Trichomonascaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>69</val></magnitude>
      <node name="g__Sugiyamaella">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>69</val></magnitude>
       <node name="s__Sugiyamaella_lignohabitans">
        <magnitude><val>69</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Schizosaccharomycetes">
    <magnitude><val>11</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Schizosaccharomycetales">
     <magnitude><val>11</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Schizosaccharomycetaceae">
      <magnitude><val>11</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Schizosaccharomyces">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>11</val></magnitude>
       <node name="s__Schizosaccharomyces_pombe">
        <magnitude><val>11</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Basidiomycota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>397</val></magnitude>
   <node name="c__Ustilaginomycetes">
    <magnitude><val>75</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Ustilaginales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>75</val></magnitude>
     <node name="f__Ustilaginaceae">
      <magnitude><val>75</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Ustilago">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>75</val></magnitude>
       <node name="s__Ustilago_maydis">
        <magnitude><val>75</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Agaricomycetes">
    <magnitude><val>14</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Agaricales">
     <magnitude><val>14</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Marasmiaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>14</val></magnitude>
      <node name="g__Marasmius">
       <magnitude><val>14</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Marasmius_oreades">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Tremellomycetes">
    <magnitude><val>308</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Tremellales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>308</val></magnitude>
     <node name="f__Cryptococcaceae">
      <magnitude><val>308</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Cryptococcus">
       <magnitude><val>308</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Cryptococcus_gattii_VGI">
        <magnitude><val>308</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
 </node>
 <node name="k__Archaea">
  <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
  <magnitude><val>2398</val></magnitude>
  <node name="p__Euryarchaeota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>2311</val></magnitude>
   <node name="c__Methanobacteria">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>155</val></magnitude>
    <node name="o__Methanobacteriales">
     <magnitude><val>155</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Methanobacteriaceae">
      <magnitude><val>155</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methanobacterium">
       <magnitude><val>25</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methanobacterium_ferruginis">
        <magnitude><val>25</val></magnitude>
       </node>
      </node>
      <node name="g__Methanobrevibacter">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>130</val></magnitude>
       <node name="s__Methanobrevibacter_sp._YE315">
        <magnitude><val>26</val></magnitude>
       </node>
       <node name="s__Methanobrevibacter_sp._AbM4">
        <magnitude><val>16</val></magnitude>
       </node>
       <node name="s__Methanobrevibacter_sp._TLL-48-HuF1">
        <magnitude><val>88</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Methanococci">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>123</val></magnitude>
    <node name="o__Methanococcales">
     <magnitude><val>123</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Methanococcaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>74</val></magnitude>
      <node name="g__Methanococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>74</val></magnitude>
       <node name="s__Methanococcus_maripaludis">
        <magnitude><val>74</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methanocaldococcaceae">
      <magnitude><val>49</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methanocaldococcus">
       <magnitude><val>49</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methanocaldococcus_infernus">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Halobacteria">
    <magnitude><val>170</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Halobacteriales">
     <magnitude><val>170</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Haloarculaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>170</val></magnitude>
      <node name="g__Halocatena">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>41</val></magnitude>
       <node name="s__Halocatena_marina">
        <magnitude><val>41</val></magnitude>
       </node>
      </node>
      <node name="g__Halomicrobium">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>106</val></magnitude>
       <node name="s__Halomicrobium_urmianum">
        <magnitude><val>106</val></magnitude>
       </node>
      </node>
      <node name="g__Halomicroarcula">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>23</val></magnitude>
       <node name="s__Halomicroarcula_marina">
        <magnitude><val>23</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Archaeoglobi">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>48</val></magnitude>
    <node name="o__Archaeoglobales">
     <magnitude><val>48</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Archaeoglobaceae">
      <magnitude><val>48</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Archaeoglobus">
       <magnitude><val>48</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Archaeoglobus_sulfaticallidus">
        <magnitude><val>48</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
   <node name="c__Methanomicrobia">
    <magnitude><val>1815</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Methanosarcinales">
     <magnitude><val>829</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Methanosarcinaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>829</val></magnitude>
      <node name="g__Methanolobus">
       <magnitude><val>49</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__uncultured_Methanolobus_sp.">
        <magnitude><val>49</val></magnitude>
       </node>
      </node>
      <node name="g__Methanimicrococcus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>13</val></magnitude>
       <node name="s__Methanimicrococcus_sp._Es2">
        <magnitude><val>13</val></magnitude>
       </node>
      </node>
      <node name="g__Methanococcoides">
       <magnitude><val>145</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methanococcoides_methylutens">
        <magnitude><val>30</val></magnitude>
       </node>
       <node name="s__Methanococcoides_burtonii">
        <magnitude><val>79</val></magnitude>
       </node>
       <node name="s__Methanococcoides_orientis">
        <magnitude><val>36</val></magnitude>
       </node>
      </node>
      <node name="g__Methanosalsum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>14</val></magnitude>
       <node name="s__Methanosalsum_zhilinae">
        <magnitude><val>14</val></magnitude>
       </node>
      </node>
      <node name="g__Methanosarcina">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>608</val></magnitude>
       <node name="s__Methanosarcina_sp._MTP4">
        <magnitude><val>145</val></magnitude>
       </node>
       <node name="s__Methanosarcina_barkeri">
        <magnitude><val>463</val></magnitude>
       </node>
      </node>
     </node>
    </node>
    <node name="o__Methanomicrobiales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>986</val></magnitude>
     <node name="f__Methanospirillaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>109</val></magnitude>
      <node name="g__Methanospirillum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>109</val></magnitude>
       <node name="s__Methanospirillum_hungatei">
        <magnitude><val>109</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methanocorpusculaceae">
      <magnitude><val>36</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methanocorpusculum">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>36</val></magnitude>
       <node name="s__uncultured_Methanocorpusculum_sp.">
        <magnitude><val>21</val></magnitude>
       </node>
       <node name="s__Methanocorpusculum_labreanum">
        <magnitude><val>15</val></magnitude>
       </node>
      </node>
     </node>
     <node name="f__Methanomicrobiaceae">
      <magnitude><val>841</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methanofollis">
       <magnitude><val>116</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Methanofollis_aquaemaris">
        <magnitude><val>116</val></magnitude>
       </node>
      </node>
      <node name="g__Methanoplanus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>725</val></magnitude>
       <node name="s__Methanoplanus_limicola">
        <magnitude><val>496</val></magnitude>
       </node>
       <node name="s__Methanoplanus_sp._FWC-SCC4">
        <magnitude><val>229</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Nitrososphaerota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>19</val></magnitude>
   <node name="c__Nitrososphaeria">
    <magnitude><val>19</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Nitrosopumilales">
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <magnitude><val>19</val></magnitude>
     <node name="f__Nitrosopumilaceae">
      <magnitude><val>19</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Nitrosopumilus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>19</val></magnitude>
       <node name="s__Nitrosopumilus_zosterae">
        <magnitude><val>19</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Candidatus_Lokiarchaeota">
   <magnitude><val>10</val></magnitude>
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <node name="c__Candidatus_Lokiarchaeia">
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <magnitude><val>10</val></magnitude>
    <node name="o__Candidatus_Prometheoarchaeales">
     <magnitude><val>10</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Candidatus_Prometheoarchaeaceae">
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <magnitude><val>10</val></magnitude>
      <node name="g__Candidatus_Prometheoarchaeum">
       <magnitude><val>10</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Candidatus_Prometheoarchaeum_syntrophicum">
        <magnitude><val>10</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Candidatus_Thermoplasmatota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>37</val></magnitude>
   <node name="c__Thermoplasmata">
    <magnitude><val>37</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Methanomassiliicoccales">
     <magnitude><val>37</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Methanomassiliicoccaceae">
      <magnitude><val>37</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Methanomassiliicoccus">
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <magnitude><val>37</val></magnitude>
       <node name="s__Candidatus_Methanomassiliicoccus_intestinalis">
        <magnitude><val>37</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
  <node name="p__Thermoproteota">
   <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
   <magnitude><val>21</val></magnitude>
   <node name="c__Thermoprotei">
    <magnitude><val>21</val></magnitude>
    <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
    <node name="o__Sulfolobales">
     <magnitude><val>21</val></magnitude>
     <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
     <node name="f__Sulfolobaceae">
      <magnitude><val>21</val></magnitude>
      <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
      <node name="g__Stygiolobus">
       <magnitude><val>21</val></magnitude>
       <magnitudeUnassigned><val>0</val></magnitudeUnassigned>
       <node name="s__Stygiolobus_azoricus">
        <magnitude><val>21</val></magnitude>
       </node>
      </node>
     </node>
    </node>
   </node>
  </node>
 </node>
</node>
  </krona>
</div></body></html>
ploading SRR14092160.krona.html…]()


## Usage:

**Data Scraping: **

Activate the Qiime2 environment and run SKINOME_training_data/data_downloader. This script will download sequencing data from skin microbiome papers listed in DataFrame_2_Pruned. DataFrame_2_Pruned was generated with code modified from the [Skinome Project](https://academic.oup.com/database/article/doi/10.1093/database/baac033/6586378). Papers were filtered to only contain microbiomes classified as healthy, atopic dermatitis, psoriasis, parapsoriasis, or acne. Papers were only included if they used swabs to collect samples and Illumina sequencing for standardization. 

**Microbiome Profile Calculation:**

Activate the Qiime2 environment and run SKINOME_training_data/QIIME2_pipeline. Ensure you have an appropriate classifier in the SKINOME_training_data/classifier folder. For more information on training a classifier, see [this guide](https://docs.qiime2.org/2024.10/tutorials/feature-classifier/). 

**Generate Diagnosis: (TODO)**

Data may lack necessary resolution for proper classification. 
