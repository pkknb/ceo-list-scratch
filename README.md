# S&P 500 公司 CEO 信息与 YouTube 视频抓取项目

这是一个自动化抓取S&P 500公司CEO信息以及CEO相关YouTube视频的项目，使用Python库如`pandas`、`yfinance`、`googleapiclient`等。项目旨在帮助用户从S&P 500公司的信息中提取CEO数据并进行相关YouTube视频的搜索与展示。

## 项目功能

1. **S&P 500公司列表抓取**：从Wikipedia抓取S&P 500公司的代码及名称。
2. **公司CEO信息获取**：通过`yfinance`库提取每家公司的CEO信息并存储到Excel文件。
3. **YouTube视频搜索**：通过YouTube API搜索每位CEO的采访视频，并保存搜索结果，包括视频标题和链接。
4. **结果存储**：抓取到的CEO信息和视频信息将保存为CSV或Excel文件。

## 使用说明

- **S&P 500公司与CEO信息抓取**：运行脚本后，程序将首先检查是否存在预先保存的Excel文件，如果不存在，将会从S&P 500列表中获取数据并调用`yfinance`库获取每家公司CEO的信息，结果会存储到本地Excel文件中。
  
- **YouTube CEO采访视频搜索**：CEO信息获取后，程序会使用YouTube API搜索与每个CEO相关的采访视频，并将结果存储在CSV文件中，供后续分析使用。

## 文件说明

- `sp500list.ipynb`: 包含项目的主要代码。
- `ceo_data.xlsx`: 用于存储CEO信息的Excel文件。
- `results.csv`: YouTube CEO采访视频搜索结果。
