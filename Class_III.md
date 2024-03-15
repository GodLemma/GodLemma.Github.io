### 序列比对
- score matrix
- (全局最优匹配)Needleman algorithm
- (局部最优匹配)Smith Waterman algorithm

### Blast
- 若使用上述算法（Needleman或者Smith），速度太慢，时间复杂度大致是平方级。
- Heuristic Methods：不用找最优而去寻找近似解
  - 寻找hits（小的相同片段），建立哈希表
  - 空间储存比对记录，用空间复杂度减小时间复杂度

### homolog
- paralogs: 相同动物的同源蛋白
- orthologs: 不同动物的同源蛋白

### Pairwise Alignment --Multiple Alignment
- HMM
- MEGA

### Projuects/Databases
