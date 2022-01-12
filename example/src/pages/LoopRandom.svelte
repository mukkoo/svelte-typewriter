<script>
	import TypewriterControls from '@example/components/TypewriterControls.svelte'
</script>

<h1>LoopRandom mode</h1>

<hr />

<pre>
  &lt;Typewriter loopRandom /&gt;
</pre>

<TypewriterControls loopRandom>
	<slot />
</TypewriterControls>

<hr />

<pre>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; /&gt;
</pre>

<TypewriterControls loopRandom interval={80}>
	<slot />
</TypewriterControls>

<hr />

<pre>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; delay=&lcub;3000&rcub; /&gt;
</pre>

<TypewriterControls loopRandom interval={80} delay={3000}>
	<slot />
</TypewriterControls>

<hr />

<pre
>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; delay=&lcub;3000&rcub; cursor=&lcub;false&rcub; /&gt;
</pre>

<TypewriterControls loopRandom interval={80} delay={3000} cursor={false}>
	<slot />
</TypewriterControls>

<hr />

<pre
>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; delay=&lcub;3000&rcub; cursor='limegreen' /&gt;
</pre>

<TypewriterControls loopRandom interval={80} delay={3000} cursor="limegreen">
	<slot />
</TypewriterControls>

<hr />

<pre>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; delay=&lcub;3000&rcub; cursor='limegreen' unwriteInterval=&lcub;20&rcub; /&gt;
</pre>

<TypewriterControls loopRandom interval={80} delay={3000} cursor='limegreen' unwriteInterval={20}>
  <slot />
</TypewriterControls>

<hr>

<pre
>
  &lt;Typewriter loopRandom interval=&lcub;80&rcub; delay=&lcub;3000&rcub; cursor='limegreen' on:done=&lcub;() =&gt; console.log('Hello World!')&rcub; /&gt;
</pre>

<TypewriterControls
	loopRandom
	interval={80}
	delay={3000}
	cursor="limegreen"
	on:done={() => console.log('Hello World!')}
>
	<slot />
</TypewriterControls>
