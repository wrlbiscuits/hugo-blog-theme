---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "快速打字"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2023-06-14T15:48:49Z
lastmod: 2023-06-14T15:48:49Z
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
```c++
#include <cstdio>
#include <string>
#include <iostream>
using namespace std;
int N;
int main(){
	scanf("%d",&N);
	for(int k = 1;k <= N;k++){
		string s1,s2;
		cin >> s1 >> s2;
		int pos = 0;
		int x = s1.size();
		int y = s2.size();
		for(int i = 0;i < y;i++){
			if(s2[i] == s1[pos]) pos++;
			if(pos == x) break;
		}
		if(pos == x) printf("Case #%d: %d\n",k,y - x);
		else printf("Case #%d: IMPOSSIBLE\n",k);
	}
	return 0;
}
```
