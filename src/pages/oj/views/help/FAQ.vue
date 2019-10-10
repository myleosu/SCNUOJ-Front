<template>
  <panel>
    <div slot="title">{{$t('m.Frequently_Asked_Questions')}}</div>
    <div class="content markdown-body">
      <ul>
        <li>输入和输出在哪里？
          <p>您的程序应从<code>stdin</code>（“标准输入”）读取输入，并将输出写入<code>stdout</code>（“标准输出”）。例如，您可以<code>scanf</code>在C或<code>cin</code>C++中使用来从stdin读取，并<code>printf</code>在C或<code>cout</code>C++中使用来写入stdout。不允许用户程序读取或写入文件，否则将显示<code>Runtime Error</code>
          </p>
        </li>
        <li>提交执行时间是什么意思？
        <p>SCNUOJ可能会使用不同的输入文件多次测试您的代码。如果您的代码在每个输入文件的时间限制内给出正确的答案，则显示的执行时间是每个测试用例所花费的最大时间。否则，执行时间将毫无意义。
        </p>
        </li>
        <li>如何使用C++ Int64？
          <p>您应声明<code>long long</code>并与<code>cin/cout</code>或者<code>%lld</code>使用，使用<code>__int64</code>将导致Compile Error。
	</p>
        </li>
        <li>Java规范？
          <p>所有程序都必须在类的静态main方法中开始<code>Main</code>。不要使用公共类：甚至<code>Main</code>必须是非公共类以避免编译错误使用缓冲<code>I/O</code>避免由于过度刷新而导致时间限制。</p>
        </li>
        <li>关于演示错误？
          <p>该oj中没有显示错误。评委将对黑色进行修整并包裹在输出的最后一行中。如果输出正确还是不一样，结果将是<code>Wrong Answer</code>。</p>
        </li>
      </ul>
    </div>
  </panel>
</template>

<script>
</script>

<style lang="less" scoped>
  .content {
    font-size: 16px;
    margin: 0 50px 40px 50px;
    > ul {
      list-style: disc;
      li {
        font-size: 16px;
        margin-top: 20px;
        &:first-child {
          margin-top: 0;
        }
        p {
          font-size: 14px;
          margin-top: 5px;
        }
      }
    }
  }
</style>
