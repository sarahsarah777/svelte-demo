<script>
	export let count;
</script>

<svg width="200" height="400" viewBox="0 0 467 667" fill="none">
	<path d="M233.333 0C388.9 203 466.667 347.433 466.667 433.333C466.667 495.217 442.083 554.566 398.325 598.325C354.566 642.083 295.217 666.667 233.333 666.667C171.449 666.667 112.1 642.083 68.3417 598.325C24.5833 554.566 0 495.217 0 433.333C0 347.433 77.7667 203 233.333 0Z" fill="#F2F2F2" fill-opacity="0.9"/>
	<mask id="mask0_3_33" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="467" height="667">
		<path d="M233.333 0C388.9 203 466.667 347.433 466.667 433.333C466.667 495.217 442.083 554.566 398.325 598.325C354.566 642.083 295.217 666.667 233.333 666.667C171.449 666.667 112.1 642.083 68.3417 598.325C24.5833 554.566 0 495.217 0 433.333C0 347.433 77.7667 203 233.333 0Z" fill="black"/>
	</mask>
	<g mask="url(#mask0_3_33)">
		<rect y={667 - (6.67*count)} width="467" height={6.67*count} fill="#008FFB"/>
	</g>
	<text text-anchor="middle" x="233.5" y="480" fill="#ffffff" font-size="180px">{count}</text>
</svg>