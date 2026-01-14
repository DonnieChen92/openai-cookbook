# Bilingual AI Application Tutorial | 双语AI应用教程

This directory contains a comprehensive tutorial for building a production-ready bilingual (Chinese-English) AI application using the OpenAI API.

本目录包含使用OpenAI API构建生产级双语（中英文）AI应用的综合教程。

## Features | 功能

### 1. Model Management | 模型管理
- Fetch and cache available OpenAI models
- Export models to CSV and Excel formats with multiple sheets
- Get model-specific parameter recommendations
- 获取并缓存可用的OpenAI模型
- 将模型导出为CSV和Excel多工作表格式
- 获取特定模型的参数推荐

### 2. Prompt Management | 提示词管理
- Save and load prompts in .txt format
- Store metadata (description, tags, timestamps)
- Import/export prompt collections as JSON
- Bilingual support for all prompts
- 以.txt格式保存和加载提示词
- 存储元数据（描述、标签、时间戳）
- 将提示词集合导入/导出为JSON
- 所有提示词支持双语

### 3. Chat Integration | 聊天集成
- Direct API calls with customizable parameters
- Use saved prompts with the OpenAI API
- Conversation history management
- Model-specific parameter optimization
- 使用可自定义参数直接调用API
- 使用保存的提示词调用OpenAI API
- 对话历史管理
- 特定模型的参数优化

## Files | 文件

- `bilingual_ai_app_tutorial.ipynb` - Main tutorial notebook | 主教程笔记本
- `requirements.txt` - Python dependencies | Python依赖项
- `README.md` - This file | 本文件

## Installation | 安装

1. Install the required packages | 安装所需的包:

```bash
pip install -r requirements.txt
```

2. Set up your OpenAI API key | 设置您的OpenAI API密钥:

```bash
export OPENAI_API_KEY="your-api-key-here"
```

Or create a `.env` file:

```
OPENAI_API_KEY=your-api-key-here
```

## Usage | 使用方法

1. Open the Jupyter notebook | 打开Jupyter笔记本:

```bash
jupyter notebook bilingual_ai_app_tutorial.ipynb
```

2. Follow the step-by-step tutorial in the notebook
   按照笔记本中的分步教程操作

3. Run each cell sequentially to understand the functionality
   依次运行每个单元格以了解功能

## Key Classes | 关键类

### PromptManager
Manages all prompt-related operations:
- `save_prompt()` - Save a prompt with metadata
- `load_prompt()` - Load a prompt from disk
- `list_prompts()` - List all available prompts
- `export_collection()` - Export all prompts to JSON
- `import_collection()` - Import prompts from JSON

管理所有提示词相关操作

### BilingualAIApp
Main application class that integrates all features:
- `initialize_models()` - Fetch and cache models
- `chat()` - Send messages to OpenAI API
- `chat_with_saved_prompt()` - Use saved prompts
- `export_models()` - Export model information
- `clear_history()` - Clear conversation history

集成所有功能的主应用类

## Code Structure | 代码结构

```
1. Dependencies Installation | 依赖安装
2. Library Imports | 库导入
3. OpenAI API Setup | OpenAI API设置
4. PromptManager Class | 提示词管理器类
5. Model Management Functions | 模型管理函数
6. BilingualAIApp Class | 双语AI应用类
7. Example Usage | 使用示例
   7.1 Initialize Application | 初始化应用
   7.2 Manage Prompts | 管理提示词
   7.3 Export Models | 导出模型
   7.4 Chat with API | 使用API聊天
   7.5 Import/Export Collections | 导入/导出集合
   7.6 Model Information | 模型信息
   7.7 Conversation History | 对话历史
8. Summary | 总结
```

## Example Outputs | 示例输出

The notebook demonstrates exporting to various formats:

- **CSV**: Simple table of models
- **Excel**: Multiple sheets with categorized models
  - All Models | 所有模型
  - GPT-4 Models
  - GPT-3.5 Models
  - Parameters | 参数推荐

- **JSON**: Prompt collections with metadata

## Requirements | 系统要求

- Python 3.8 or higher | Python 3.8或更高版本
- OpenAI API key | OpenAI API密钥
- Internet connection for API calls | 用于API调用的互联网连接

## Notes | 注意事项

- Some cells require a valid OpenAI API key to execute
- Model caching reduces API calls and improves performance
- All exports use UTF-8 encoding for proper bilingual support
- Conversation history can be cleared to start fresh conversations

- 某些单元格需要有效的OpenAI API密钥才能执行
- 模型缓存可减少API调用并提高性能
- 所有导出都使用UTF-8编码以正确支持双语
- 可以清除对话历史以开始新的对话

## Customization | 自定义

You can easily extend this application:

1. Add more model-specific parameters
2. Implement streaming responses
3. Create custom prompt templates
4. Add support for other OpenAI services (DALL-E, Whisper)
5. Build a web interface

您可以轻松扩展此应用程序

## License | 许可证

This tutorial is part of the OpenAI Cookbook and follows the same license.

本教程是OpenAI Cookbook的一部分，遵循相同的许可证。

## Support | 支持

For issues or questions:
- Check the [OpenAI Documentation](https://platform.openai.com/docs)
- Visit the [OpenAI Community Forum](https://community.openai.com)

有关问题或疑问：
- 查看OpenAI文档
- 访问OpenAI社区论坛
