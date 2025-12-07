# Dome Gallery

A 3D spherical/dome image gallery with drag controls and image enlargement.

## Installs

```bash
npm install @use-gesture/react
```

## Usage

```jsx
import DomeGallery from './DomeGallery';

const images = [
  'img1.jpg', 'img2.jpg', 'img3.jpg'
];

const Example = () => {
  return (
    <div style={{ height: '100vh', width: '100vw' }}>
      <DomeGallery 
        images={images}
        segments={20}
        minRadius={600}
      />
    </div>
  );
};

export default Example;
```

## Props

| Prop | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `images` | `array` | `[...]` | Array of image URLs or objects (`{src, alt}`). |
| `fit` | `number` | `0.5` | Scales the radius relative to viewport. |
| `minRadius` | `number` | `600` | Minimum radius of the dome. |
| `maxRadius` | `number` | `Infinity` | Maximum radius of the dome. |
| `segments` | `number` | `35` | Number of columns in the dome grid. |
| `overlayBlurColor` | `string` | `'#060010'` | Backdrop color when image is enlarged. |
| `enlargeTransitionMs` | `number` | `300` | Transition duration for enlargement. |
| `imageBorderRadius` | `string` | `'30px'` | Border radius for gallery tiles. |
